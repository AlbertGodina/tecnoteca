# Tecnoteca

Guia de Tecnologia i Digitalització per a l'ESO. Web feta amb [MkDocs Material](https://squidfunk.github.io/mkdocs-material/), en català, llicència CC BY-SA 4.0.

## Provar-la en local

```bash
pip install -r requirements.txt
mkdocs serve
```

Obre <http://127.0.0.1:8000>.

## Estructura

- `docs/1r`, `2n`, `3r`, `4t`: rutes per curs (unitats i tasques).
- `docs/banc`: banc temàtic compartit (teoria que enllacen les tasques).
- `docs/eines`: simuladors i exercicis interactius.
- `plantilles/tasca.md`: plantilla de pàgina de tasca (no es publica).
- `docs/stylesheets/tecnoteca.css`: colors i estil (mode clar i fosc).

Per afegir una pàgina: crea el `.md` dins de `docs/` i afegeix-lo a `nav` de `mkdocs.yml`.

## Publicar a GitHub Pages

1. Crea el repositori `tecnoteca` a GitHub i puja-hi aquest contingut a la branca `main`.
2. Substitueix `USUARI` a `mkdocs.yml` pel teu usuari o organització.
3. Cada `push` a `main` executa `.github/workflows/deploy.yml` i publica a la branca `gh-pages`.
4. A *Settings › Pages*, tria com a font la branca `gh-pages`.


