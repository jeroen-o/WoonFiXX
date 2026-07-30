# WoonFiXX Hypotheken — Website

Statische website voor **woonfixx.nl**, gehost op GitHub Pages.

## Stack

- Pure HTML / CSS / vanilla JavaScript — geen build-stap
- DM Sans (via Google Fonts)
- SVG logo's en iconen
- Mobile-first responsive

## Structuur

```
.
├── index.html                  Homepage
├── aanpak.html                 Methodologie (PARP / POG)
├── diensten.html               Productontwikkeling + consultancy + sectoren
├── initiatieven.html           Eigen proposities in ontwikkeling
├── over-ons.html               Verhaal, principes, Jan Boers
├── contact.html                Contactgegevens + formulier + map
├── 404.html                    404-pagina
├── CNAME                       Custom domein voor GitHub Pages
├── assets/
│   ├── logo.svg                Horizontaal logo (navy plate, oranje accent)
│   └── logo-stacked.svg        Vierkant/avatar variant
├── css/
│   └── styles.css              Volledige stylesheet
└── js/
    └── script.js               Mobiel menu, accordeon, reveal-animaties, formulier
```

## Deployment naar GitHub Pages

1. Push deze map naar de `main` branch van een GitHub-repo.
2. Repository → Settings → Pages → Source: `Deploy from a branch` → Branch: `main` → Folder: `/ (root)`.
3. Wacht tot de site live staat.

### Custom domein (woonfixx.nl)

De `CNAME` file regelt het automatisch. Bij de DNS-provider:

**A-records voor het apex-domein:**
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME voor `www`:**
```
www  →  <user>.github.io
```

In Repository Settings → Pages: zet **Enforce HTTPS** aan zodra het certificaat is uitgegeven.

## License

© WoonFiXX Hypotheken — KvK 09190751
