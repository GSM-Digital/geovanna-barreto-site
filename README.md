# Geovanna B Nutri — Site

Site one-page de **Geovanna Barreto**, nutricionista comportamental (Goiânia + online).

- **Produção:** https://geovannabnutri.com.br/
- **Stack:** HTML + CSS + JS estáticos (sem frameworks). Todo o CSS e JS estão inline no `index.html`.
- **Deploy:** cPanel → Git Version Control (HostGator). O `.cpanel.yml` copia os arquivos para o document root a cada `git push`.

## Estrutura

```
index.html          → página completa (HTML + CSS + JS inline)
.htaccess           → gzip + cache de 1 ano para assets estáticos
.cpanel.yml         → script de deploy automático do cPanel
assets/
  geovanna-1..3.webp  → fotos
  local-1..2.webp     → mapas dos consultórios
  logo-2.svg          → logo branca (rodapé)
  logo-3.svg          → logo verde (menu)
  favicon.svg         → favicon adaptativo (claro/escuro)
  fonts/*.woff2       → DM Sans + Playfair Display (subsets latin/latin-ext)
```

## Como atualizar o site

1. Editar os arquivos localmente.
2. `git add . && git commit -m "descrição" && git push`
3. No cPanel → Git Version Control → **Update from Remote** → **Deploy HEAD Commit**.

Desenvolvido por [Thiago Barreto](https://thbarreto.com.br/).
