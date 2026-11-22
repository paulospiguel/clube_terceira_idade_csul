# Clube da Terceira Idade CSUL — Contexto do domínio

Público: Brasil, pt-BR (ver docs/adr/0001).

Glossário vivo. Atualizado durante a sessão de planeamento. Termos marcados _(provisório)_ ainda não foram confirmados.

## Pessoas

- **Visitante** — qualquer pessoa que abre o site público sem iniciar sessão.
- **Sócio** — membro do clube. Não tem conta no site (ADR 0002).
- **Gestor** — membro do conselho/diretoria com login no painel. Publica conteúdo e gere a Agenda. _(perfis e permissões por definir)_
- **Órgãos sociais** — Diretoria e Conselho, mostrados numa página própria. _(nomes exatos dos órgãos por confirmar)_

## Conteúdo

- **Evento** — algo com data, hora e local que aparece na Agenda (ex.: baile, passeio, aula).
- **Agenda** — lista cronológica de Eventos futuros e passados.
- **Publicação** — notícia ou post escrito no painel.
- **Feed social** — publicações do Instagram/Facebook do clube, incorporadas (embed), não importadas (ADR 0003).
- **Galeria** — fotos de Eventos.
- **Prestação de contas** — documentos e registos de receitas/despesas publicados no site. Pública para qualquer Visitante (ADR 0007).

## Contacto

- **Pedido de contacto** — mensagem enviada pelo formulário geral, entregue por e-mail (ADR 0004).
- **Proposta de atuação** — pedido de uma banda/artista para tocar num dia específico, entregue por e-mail.
- **Contacto rápido** — botão de WhatsApp.

## Infraestrutura

- **Armazenamento de ficheiros** — Cloudflare R2 (documentos, fotos, imagens).
- **Aplicação** — Node.js na Vercel, Postgres gratuito (Neon ou Supabase) (ADR 0005).
