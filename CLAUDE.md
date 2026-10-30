# SAVA — Landing do anúncio, versão 2 (lp2)

Página única (`index.html`, tudo embutido, sem build). Publicada pelo GitHub Pages em
https://lp2.savatecnologia.com.br (arquivo `CNAME`). Todo push na `main` publica.
A versão 1 mora em `Pedrobonanno1/sava-landing` (lp.savatecnologia.com.br).

- Origem: `sava-landing-anuncio-2026-10-27.html`, prévia gerada de
  `LINA Code/landing-anuncio-2026-10-26/index.html` (fonte não encontrada nesta máquina nem no
  GitHub em 30/10/2026). Removida a linha `window.SAVA_PREVIA = true` para o form gravar.
- O formulário grava na tabela `inscricoes` do Supabase da SAVA Gestão
  (`lina-gestao/supabase/inscricoes.sql`). A chave `anon` no HTML é pública por desenho.
- Nunca publicar com `<script>window.SAVA_PREVIA = true</script>` (form não grava).
- Pixel da Meta: preencher `META_PIXEL_ID` no `index.html` (vazio = não carrega).

## Git: absolutamente tudo é salvo — commit E push — sem perguntar

- Toda mudança que deixa o projeto funcionando vira **commit e push** na mesma sessão, logo
  depois de feita. Não perguntar "quer que eu faça o commit?".
- **Nunca** vai pro git: segredo e credencial (`.env`, `*.local`, chaves, tokens), dado real
  de cliente.
- Ainda pedir confirmação antes de: force-push, reescrever histórico, apagar branch.
- Aqui push na `main` = publicar em produção; o Pedro pediu a publicação em 30/10/2026, mas
  mudança grande de conteúdo/oferta: mostrar antes.
