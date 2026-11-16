# Changelog

Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/) e [SemVer](https://semver.org/lang/pt-BR/).

## [0.5.0] — 2026-11-16
### Adicionado
- Topo com o problema na frente (“Praga em casa ou portão travado?”), duas portas de entrada (pragas 24h / reparos com agendamento), botões Orçamento, Ligar agora e WhatsApp, e faixa de confiança (nota Google, dedetização 24h, garantia, orçamento em PDF).
- Seção **Qual é o problema?** com abas Pragas e Reparos: um toque preenche o pedido de orçamento.
- Bloco **Achou escorpião em casa?** com primeiros passos, CIATox-DF (0800 644 6774) e SAMU (192).
- Seção **Veja como é o nosso orçamento**: exemplo de orçamento técnico e de proposta de dedetização (cliente fictício, valores ilustrativos).
- Seção **Garantia por escrito** com botão para acionar a garantia.
- Seção **Como se preparar** (antes e depois da dedetização).
- Barra fixa no celular com Ligar e WhatsApp; botão Ligar no cabeçalho.
- Regiões atendidas, aviso de época (set–mar) e marcação de perguntas frequentes para o Google.
- Novas perguntas: preço, comprovante, 24h, material, portão industrial.
### Alterado
- “Atendimento 24 horas” passa a valer só para dedetização; reparos e instalações “com agendamento”.
- Diferenciais reescritos: garantia por escrito, orçamento detalhado, dedetização 24h, técnico identificado.

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
