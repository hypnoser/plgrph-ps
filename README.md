# Polygraph Suite — ps.plgrph.com

Статичний застосунок (без збірки, без серверної частини). Хостинг: GitHub Pages (Deploy from a branch → `main` / root), DNS: Cloudflare (`ps` → CNAME на `hypnoser.github.io`).

## Структура
- `index.html`, `en/`, `es/` — калькулятор (uk/en/es); `info.html`, `en/info.html`, `es/info.html` — довідка
- `pr/`, `pr/en/`, `pr/es/` — презентація застосунку для нових користувачів
- `js/`, `lang/`, `css/` — код і переклади; `assets/` — шрифти та зображення, спільні для презентацій

## Правила
- Файли калькулятора не змінювати без потреби: дані користувачів лежать у localStorage/IndexedDB цього origin (`polygraph_suite_data`, `suite_auth`, IndexedDB для нотаток).
- Шрифти — self-hosted (`/assets/fonts/`), зовнішніх CDN немає (крім Google Analytics G-Q7JS2JHVG7).
- Canonical-адреси: `https://ps.plgrph.com/...`; зміна домену потребує заміни в `pr/*`, `sitemap.xml`, `robots.txt`, `CNAME`.
