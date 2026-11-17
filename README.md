# SmartLar — Site e App de Orçamentos

Site da **SmartLar** (Dedetização e Desratização · Serviços & Segurança) e o app interno de orçamentos, no mesmo repositório.

```
/            → site público (index.html + assets/)
/app/        → app de orçamentos da equipe (um único index.html, funciona offline)
```

## Publicar no GitHub Pages
1. No repositório: **Settings → Pages → Build and deployment → Deploy from a branch**.
2. Escolha a branch `main` e a pasta `/ (root)` → **Save**.
3. Em alguns minutos o site fica em `https://<seu-usuario>.github.io/<repositório>/` e o app em `.../app/`.
4. Para usar um domínio próprio (ex.: `smartlardf.com.br`), configure em **Settings → Pages → Custom domain**.

> GitHub Pages em repositório **privado** exige plano pago do GitHub. No plano gratuito, o repositório precisa ser público para publicar.

## Ajustes rápidos no site
- **Regiões atendidas:** lista `REGIOES` no fim do `index.html`.
- **Aviso de época** (escorpiões e baratas): aparece de setembro a março; o visitante pode fechar.
- **Atendimento 24 h:** vale só para dedetização. Reparos e instalações aparecem como "com agendamento".

## Google Meu Negócio no site
Sem configuração, o site mostra a nota e o total de avaliações gravados em `GOOGLE` (no fim do `index.html`). Atualize `rating`, `total` e `conferidoEm` a cada versão.

Para sincronizar automaticamente (nota, total e até 3 avaliações recentes de 4–5 estrelas):
1. No [Google Cloud Console](https://console.cloud.google.com/), crie um projeto e ative a **Places API (New)**. É preciso uma conta de faturamento; há uma cota mensal gratuita.
2. Crie uma **chave de API** e restrinja: *Restrições de aplicativo → Referenciadores HTTP* com o endereço do site (ex.: `https://usuario.github.io/*`) e *Restrições de API → Places API (New)*.
3. Cole a chave em `GOOGLE.apiKey`. O `placeId` é opcional (o site busca pelo nome). As respostas ficam em cache por 12 h no navegador do visitante.

## App de orçamentos
- Abra `app/index.html` no navegador (ou pelo endereço do Pages + `/app/`).
- Configure em **Mais → Empresa, perfis e padrões**.
- PDF: botão **PDF → Imprimir → Salvar como PDF**.
- Os dados ficam **no aparelho** (localStorage). Faça backup em **Mais → Backup**.
- **Nunca** suba backups, fotos ou dados de clientes para este repositório.

## Versões
Cada versão tem uma etiqueta (`git tag`) no formato `vMAIOR.MENOR.CORREÇÃO`. Detalhes no [CHANGELOG](CHANGELOG.md).

| Etiqueta | Conteúdo |
|---|---|
| `v0.1.0` | App: orçamentos, clientes, dois perfis de marca, PDF e WhatsApp |
| `v0.2.0` | App: identidade visual e PDF no modelo oficial da SmartLar |
| `v0.3.0` | Site institucional + pedido de orçamento pelo WhatsApp; app movido para `/app` |
| `v0.4.0` | Site: avaliações e mapa do Google Meu Negócio |
| `v0.5.0` | Site: "Qual é o problema?", ligar + barra fixa no celular, exemplo de orçamento, garantia, escorpião, preparo, regiões |
| `v0.6.0` | Site enxuto (7 blocos, sem portão) + conteúdo editável pela planilha do Google (ver `docs/PLANILHA.md`) |
| `v0.6.1` | Site ligado à planilha do Google |
| `v0.6.2` | Site só de dedetização (serviços da casa ficam no app de orçamento) |
| `v0.7.0` *(planejada)* | App: produtos químicos, registro de serviço, relatório + recibo |
| `v0.8.0` *(planejada)* | App: retornos automáticos (garantia e próxima aplicação) |
| `v0.9.0` *(planejada)* | App: assinatura na tela, fotos, checklist de ambientes e cartaz de aviso |
| `v0.10.0` *(planejada)* | Site ↔ app: pedidos do site entram direto no app |
