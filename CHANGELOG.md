# Changelog

Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/) e [SemVer](https://semver.org/lang/pt-BR/).

## [0.4.0] — 2026-11-14
### Adicionado
- Seção **Avaliações** com a nota do Google (4,9 · 40 avaliações em 14/11/2026), botões “Avaliar a SmartLar” e “Ver todas no Google”.
- Selo da nota do Google no topo do site e item “Avaliações” no menu.
- Mapa do Google Maps incorporado (sem chave).
- Sincronização opcional via Places API (New): nota, total, até 3 avaliações recentes (4–5★) com atribuição ao Google e link direto de “escrever avaliação”; cache de 12 h.

## [0.3.0] — 2026-11-14
### Adicionado
- Site institucional (`/`) com a identidade das artes: hero, as duas frentes de serviço, diferenciais, como funciona, dúvidas frequentes e rodapé.
- Formulário de orçamento que monta a mensagem e abre o WhatsApp (sem guardar dados no site).
- Botão flutuante de WhatsApp, link para o Google Maps, dados estruturados (SEO local) e imagem de compartilhamento.
- Ícones, favicon e logo em `assets/`.
### Alterado
- App de orçamentos movido para `/app/` (dados salvos no aparelho continuam valendo no mesmo endereço).

## [0.2.0] — 2026-11-14
### Adicionado
- Identidade visual: logo oficial embutida, cabeçalho escuro, laranja (Dedetização) e azul (Serviços & Segurança), fonte Poppins.
- PDF no modelo oficial da SmartLar: logo em todas as páginas, tabelas Cliente / Empresa, detalhamento numerado, cláusulas com destaque em vermelho (prefixo `!`), garantia, condições de pagamento.
- Proposta de dedetização com tabela de tipo de imóvel, foco, observação de execução, valor por serviço e validade por extenso.
- Título do serviço (ex.: “Troca de caixa d'água”).
- Lista de materiais com foto e quantidade; materiais usados ficam salvos com a foto para os próximos orçamentos.
- Mão de obra + materiais separados; valor à vista por % ou valor fechado (ex.: R$ 1.800,00).
- Botão “Duplicar” orçamento.
### Alterado
- Catálogo de Serviços & Segurança alinhado às artes (motor de portão residencial e industrial, troca de caixa d'água).
- Dados salvos na v0.1.0 são migrados automaticamente.

## [0.1.0] — 2026-11-13
### Adicionado
- Orçamentos com tipo de imóvel, pragas-alvo, área, itens do catálogo ou livres, desconto no PIX, parcelamento e validade.
- Status do orçamento: aberto, aprovado, recusado.
- Documento em PDF (via Imprimir) com valor por extenso e validade.
- Mensagem pronta para WhatsApp com itens, total e valor no PIX.
- Clientes com ficha e histórico de orçamentos; cadastro rápido dentro do orçamento.
- Dois perfis de marca: Dedetização e Serviços & Segurança (cor, logo, catálogo, textos).
- Início com indicadores do mês e lembrete de orçamentos perto de vencer.
- Backup e restauração em arquivo JSON.
