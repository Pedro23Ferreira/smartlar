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
| `v0.4.0` *(planejada)* | App: produtos químicos, registro de serviço, relatório + recibo |
| `v0.5.0` *(planejada)* | App: retornos automáticos (garantia e próxima aplicação) |
| `v0.6.0` *(planejada)* | App: assinatura na tela, fotos, checklist de ambientes e cartaz de aviso |
| `v0.7.0` *(planejada)* | Site ↔ app: pedidos do site entram direto no app |
