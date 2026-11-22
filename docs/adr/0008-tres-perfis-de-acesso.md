# 0008 — Três perfis de acesso no painel

**Estado:** aceite (2026-11-22)

## Decisão
| Perfil | Pode gerir |
|---|---|
| Administrador | Tudo, incluindo contas de outros Gestores |
| Editor | Agenda, Publicações, Galeria, Órgãos sociais |
| Tesoureiro | Prestação de contas |

Uma conta tem um perfil. Registo de autoria (quem criou/alterou e quando) obrigatório na Prestação de contas. _(assumido pela recomendação; o Paulo não contestou)_

## Consequências
- Autorização verificada no servidor em cada ação, não só escondendo botões.
- Um Administrador inicial é criado no primeiro deploy (seed).
