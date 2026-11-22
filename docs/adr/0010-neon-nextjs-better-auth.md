# 0010 — Neon como base de dados, Next.js e Better Auth

**Estado:** aceite (2026-11-22). Completa o ADR 0005.

## Decisão
- Postgres no Neon (plano gratuito).
- Next.js (App Router) na Vercel, para site público e painel na mesma aplicação.
- Login por e-mail e senha com Better Auth, contas guardadas no Neon.

## Porquê não Supabase
O plano gratuito do Supabase pausa projetos inativos e exige reativação manual ([docs](https://supabase.com/docs/guides/platform/free-project-pausing)). O storage e o login do Supabase trariam pouco, porque os ficheiros já vão para o R2.

## Consequências
- O Neon suspende o compute sem uso. O primeiro acesso depois disso tem alguns segundos de atraso. Páginas públicas devem ser geradas estaticamente/em cache (ISR) para o Visitante não sentir isto.
- Limites do plano gratuito a acompanhar: https://neon.com/docs/introduction/plans
