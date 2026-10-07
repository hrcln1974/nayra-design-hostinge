# Salão Nayra Design — Hostinger

## Hospedagem
Este pacote é preparado para hospedagem estática na Hostinger. Não depende de Node.js para o site público.

### Publicação
1. Abra o Gerenciador de Arquivos da Hostinger.
2. Entre em `public_html`.
3. Envie o conteúdo desta pasta (e não a pasta contêiner) para `public_html`.
4. Confirme que `index.html`, `.htaccess`, `robots.txt` e `sitemap.xml` estão na raiz.
5. Ative o SSL/HTTPS da Hostinger.

### Firebase
O agendamento dinâmico e o painel administrativo usam Firebase. Antes da entrega operacional, preencha `firebase-config.js` com o projeto Firebase do cliente e repita os testes. As credenciais de navegador não são segredos; regras do Firestore/Storage devem restringir acesso.

### URLs
- Site: `/`
- Obrigado: `/obrigado.html`
- Privacidade: `/privacidade.html`
- Painel: `/admin-salao/`
- Agendamento/painel alternativo: `/admin-agendamento/`

### Google
Após apontar o domínio: valide propriedade no Search Console, envie `/sitemap.xml`, verifique indexação e configure GA4 quando o cliente fornecer o ID.
