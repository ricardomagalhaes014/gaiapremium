# Gaia Premium — Landing page

Site de apresentação do empreendimento **Gaia Premium** (Vila Nova de Gaia), com a **dps Imobiliário**.

Site estático (HTML + CSS + JS, sem dependências de build). Pensado para ser publicado em:

```
https://dpsimobiliario.pt/gaiapremium
```

## Estrutura

```
gaiapremium/
├── index.html
├── assets/
│   ├── css/style.css
│   ├── js/main.js
│   ├── logo-dps.svg
│   └── img/            (renders e fotos do empreendimento)
├── robots.txt
└── README.md
```

Todos os caminhos são **relativos**, por isso o site funciona tanto em subpasta (`/gaiapremium`) como num domínio próprio.

## Publicar via GitHub

1. Criar um repositório (ex.: `gaiapremium`) e enviar estes ficheiros:
   ```bash
   cd gaiapremium
   git init
   git add .
   git commit -m "Gaia Premium landing page"
   git branch -M main
   git remote add origin https://github.com/<utilizador>/gaiapremium.git
   git push -u origin main
   ```
2. Colocar o conteúdo na pasta `/gaiapremium` do site `dpsimobiliario.pt` (via FTP, painel de hosting, ou GitHub Pages + redirecionamento).

## Notas importantes

- **Sem contactos do promotor.** O único contacto presente é o da dps Imobiliário: WhatsApp **925 610 864** (botão lateral fixo + formulário).
- O formulário de contacto abre uma conversa de WhatsApp já preenchida (não precisa de servidor/backend).
- O logótipo `logo-dps.svg` é uma reprodução vetorial dourada. Para usar o ficheiro original da marca, substituir `assets/logo-dps.svg` mantendo o mesmo nome.
- Imagens 3D meramente indicativas, extraídas da brochura do empreendimento.
- Mapa: centrado em Vila Nova de Gaia. Para apontar à morada exata, editar o `src` do `<iframe>` em `index.html` (secção Localização).
