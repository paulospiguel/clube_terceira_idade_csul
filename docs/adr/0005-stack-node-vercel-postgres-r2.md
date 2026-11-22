# 0005 — Node.js na Vercel, Postgres gratuito, ficheiros no Cloudflare R2

**Estado:** aceite em princípio (2026-11-22). Escolha Neon vs Supabase em aberto.

## Decisão
Aplicação Node.js publicada na Vercel. Dados em Postgres de plano gratuito (Neon ou Supabase). Documentos e fotos no Cloudflare R2.

## Consequências
- Uploads diretos do navegador para o R2 via URLs pré-assinadas (evita limite de tamanho das funções da Vercel).
- Planos gratuitos têm limites (pausa por inatividade, armazenamento) a confirmar.
