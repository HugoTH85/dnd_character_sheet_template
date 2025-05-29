# Gestion de la fiche de personnage

## Prérequis

- Installer Quarto CLI : [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)

- Sur Visual Studio Code, installer l'extension Quarto

## Utilisation du projet

1. Un fichier .qmd équivaut à une page

2. Chaque fichier `.qmd` doit commencer par cette section :

```markdown
---
title: "Titre de la page"
format:
  html:
    css: styles.css
    theme: cosmo
---
```

3. Le contenu d'une page doit être inséré dans la balise html suivante :

```html
<div class="phb">
your content in markdown
</div>
```

4. Après création d'une nouvelle page, rdv dans le fichier `_quarto.yml` pour l'intégrer à la navbar. Ajouter ces lignes dans la section `left` :

```yaml
- href: your_file.qmd
  text: Nom_de_la_page
```

5. Pour voir le rendu du projet, faites `ctrl+shift+k` ou exécutez la commande `quarto preview` dans un terminal à la racine du projet
