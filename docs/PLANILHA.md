# Como editar o site pela planilha

O texto do site que muda com frequência fica numa planilha do Google ("SmartLar - Conteúdo do site").
Quem tem acesso à planilha edita ali, sem mexer em código. O site atualiza sozinho em alguns minutos.

## O que dá para mudar

| Seção | Campos |
|---|---|
| Contato | telefone (como aparece e o do botão Ligar), WhatsApp, CNPJ |
| Aviso de época | faixa no topo: modo (AUTO / SIM / NAO), texto e botão |
| Avaliações Google | nota e total de avaliações |
| Licenças | licença sanitária, licença ambiental e responsável técnico (vazio = não aparece) |
| Orçamento de exemplo | mostrar ou esconder valores (SIM / NAO) e os valores da dedetização |
| Regiões atendidas | uma linha por região (apague a linha para tirar; adicione outra com Campo = `regiao`) |

Só a coluna **Valor** deve ser alterada. A coluna **Campo** é o nome que o site procura: não mude.

## Regras rápidas

- Valores em reais: pode digitar `1.953,00` ou `1953`.
- Nota: com ponto (`4.9`) ou vírgula (`4,9`).
- Campo vazio = o site mantém o texto que já tem.
- Se a planilha sair do ar, o site continua normal com os últimos textos.

## Ligar o site à planilha (já está ligado)

1. Na planilha: **Compartilhar > Acesso geral > Qualquer pessoa com o link > Leitor**.
2. O link usado pelo site é este (troque `ID_DA_PLANILHA` e `NUMERO_DA_ABA` pelos da sua planilha; o número da aba está no fim do endereço, depois de `gid=`):
   `https://docs.google.com/spreadsheets/d/ID_DA_PLANILHA/gviz/tq?tqx=out:csv&headers=1&gid=NUMERO_DA_ABA`
3. Ele fica em `index.html`, na linha `const PLANILHA = { csv: "...", ... }`.

Para parar de usar a planilha, deixe o link vazio (`csv: ""`) e envie para o GitHub.

## Limites

- Nome da empresa, pragas atendidas, FAQ e textos longos ficam no código (`index.html`).
- O Google (busca) lê o texto que está no código, não o que vem da planilha. Mantenha telefone e regiões
  do código atualizados de vez em quando.
- A planilha fica aberta para leitura por quem tiver o link. Não coloque nada confidencial nela.
