## A) Taille de texte : `px` et `rem` manquants

Actuellement :

* `em` utilisé (`1.4em`) ✅

À ajouter :

* un `px`
* un `rem`

Exemple :
```
h1 {
font-size: 32px;
}

p {
font-size: 1rem;
}
```

💡 *L’exercice demande les 3 unités pour comprendre leurs différences.*

---

## B) Largeur maximale + centrage horizontal manquants

Actuellement :
```
body {
max-width: 100%;
}
```

Problème :

* `max-width: 100%` ne limite rien (c’est la largeur normale)
* la page n’est pas “contenue” dans 800px

À corriger (exemple simple) :
```
main {
max-width: 800px;
margin: 0 auto;
}
```

💡 *Limiter la largeur rend la lecture plus confortable.*

> *Une ligne de texte trop longue est plus difficile à lire.*

---

## C) Police personnalisée : déclarée mais pas utilisée

Vous avez bien un `@font-face`, mais aucune règle ne l’applique.

À ajouter :
```
body {
font-family: "Tagesschrift", Arial, sans-serif;
}
```

💡 *Déclarer une police ne suffit pas : il faut l’appliquer à un élément.*

De plus, n'oubliez pas de l'importer dans un fichier dossiers `/fonts`

---

## D) Amélioration CSS (optionnel mais conseillé) : images fluides

Actuellement :

* pas de règle “responsive” globale pour les images

À ajouter :
```
img {
max-width: 100%;
height: auto;
}
```

💡 *Cela évite que l’image dépasse du bloc sur mobile.*

---

## Corrections HTML nécessaires (impact CSS)

### 1️⃣ Trop de `<br>` dans le HTML

Vous utilisez plusieurs `<br>` pour créer de l’espace.

À corriger :

* supprimer les `<br>`
* gérer l’espacement en CSS, par exemple :
  ```
  h2 {
  margin-top: 20px;
  }
  ul {
  margin-bottom: 20px;
  }
  ```

💡 *Les espacements doivent être gérés en CSS, pas avec `<br>`.*

> *Le HTML = structure, le CSS = mise en forme.*

---

### 3️⃣ Image de profil cliquable

Lien actuel :
```
<a href="#" class="logo">
```

À corriger :

* le clic doit ouvrir l’image dans un nouvel onglet :
```
  <a href="./img/profile.png" target="_blank" rel="noopener noreferrer" class="logo">
  <img src="./img/profile.png" alt="Photo de profil de Pierre-Alexandre">

</a>
```

💡 *`rel="noopener noreferrer"` évite qu’un onglet externe puisse manipuler la page d’origine.*

---
