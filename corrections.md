## A) Dossier CSS et liens vers les fichiers (normalize + main)
- Veuillez utiliser un dossier `css/` (en minuscules) comme demandé
- `normalize.css` doit être en local dans `./css/normalize.css`
- Exemple attendu dans le `<head>` :
```
<link rel="stylesheet" href="./css/normalize.css">
<link rel="stylesheet" href="./css/main.css">
```

## B) Image du header : dossier `img/` + lien cliquable correct
- Veuillez mettre l’image dans `./img/`
- Le clic doit ouvrir l’image dans un nouvel onglet
- Exemple :
```
<a href="./img/Profile.png" target="_blank" rel="noopener noreferrer">
  <img src="./img/Profile.png" alt="Photo de Pierre-Alexandre">
</a>
```
## C) Corriger les `id` (bonne pratique)
- Veuillez utiliser des `id` simples, en minuscules, sans accents, sans espaces
- Exemple : `experience`, `competences`, `formation`
- Et mettre à jour les liens du menu (`href="#..."`)

## D) Footer : ajouter l’e-mail en `mailto:`
- Veuillez afficher votre e-mail dans le footer et le rendre cliquable
- Exemple :
```
<footer>
  &copy;2025 Pierre-Alexandre —
  <a href="mailto:prenom.nom@email.com">prenom.nom@email.com</a>
</footer>
```

## Autres
- Attention à l'indentation et à la lisibilité du code
- description dans le `<head>`
- manque les favicon dans la racine, ou alors adapter le chemin dans `index.html`
