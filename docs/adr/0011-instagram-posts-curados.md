# 0011 — Feed social: Facebook Page Plugin e posts do Instagram escolhidos no painel

**Estado:** aceite (2026-11-22). Detalha o ADR 0003.

## Decisão
- Facebook: widget oficial Page Plugin da página do clube (sem token).
- Instagram: o Editor cola no painel o link de um post; o site mostra o embed oficial desse post. Ordem e remoção geridas no painel.

## Consequências
- Sem custos nem tokens a expirar.
- Não atualiza sozinho: depende de o Editor adicionar posts.
- Embeds da Meta carregam scripts de terceiros (afeta desempenho e privacidade). Carregar só quando a secção do feed fica visível.
