# mysamplespringbootNoOpt
My  Sample Spring boot no Opt 

Voici une liste des modifications apportées à **chaque fichier HTML dégradé**, avec des explications sur ce qui a été changé et comment revenir à la version originale.

---

## **HTML 1 : Page d'accueil**
### Modifications
1. **Ajout de scripts et liens CSS inutiles :**
    - Scripts et styles ajoutés qui ne sont pas utilisés.
    - Rendent le chargement plus lourd.

2. **Ajout de longues balises `<div>` inutiles :**
    - Structures HTML imbriquées sans raison.

3. **Duplication de contenu dans le `<header>` et le `<footer>` :**
    - Le contenu a été répété inutilement.

4. **Balises non nécessaires dans la section principale :**
    - Des éléments comme des images ou des `<div>` avec du texte aléatoire ont été ajoutés.

### Comment revenir à la version originale ?
1. Supprimez tous les scripts et liens CSS ajoutés inutilement.
2. Réduisez la structure HTML en supprimant les `<div>` imbriqués superflus.
3. Éliminez les duplications dans le `<header>` et le `<footer>`.
4. Enlevez tout contenu supplémentaire qui ne figure pas dans le fichier d'origine.

---

## **HTML 2 : Liste des produits**
### Modifications
1. **Ajout de styles inutiles dans `<head>` :**
    - Fichiers CSS supplémentaires qui ne sont pas utilisés.

2. **Ajout de lignes `<tr>` et `<td>` supplémentaires vides dans le tableau :**
    - Ces lignes rendent le tableau inutilement long.

3. **Ajout d’attributs inutiles sur les balises :**
    - Exemple : Ajout d’attributs comme `style` avec des valeurs redondantes.

4. **Répétition de liens dans le menu `<nav>` :**
    - Duplication de liens déjà présents.

5. **Ajout d’images inutiles et d’espaces vides :**
    - Images aléatoires ajoutées pour alourdir la page.

### Comment revenir à la version originale ?
1. Supprimez les fichiers CSS et les `<style>` non nécessaires.
2. Retirez les lignes vides `<tr>` et `<td>` du tableau.
3. Nettoyez les balises en enlevant les attributs redondants ou inutiles.
4. Éliminez les duplications dans le menu `<nav>`.
5. Supprimez les images superflues et les éléments vides.

---

## Plan pour Revenir à la Version Originale (Code Exemple)

### Exemple : Page d'accueil simplifiée
#### Code actuel (dégradé)
```html
<header>
    <nav>
        <ul>
            <li><a href="/">Accueil</a></li>
            <li><a href="/products">Produits</a></li>
            <li><a href="/products/new">Nouveau Produit</a></li>
        </ul>
    </nav>
</header>
<header>
    <nav>
        <ul>
            <li><a href="/">Accueil</a></li>
            <li><a href="/products">Produits</a></li>
            <li><a href="/products/new">Nouveau Produit</a></li>
        </ul>
    </nav>
</header>
```

#### Code d'origine
```html
<header>
    <nav>
        <ul>
            <li><a href="/">Accueil</a></li>
            <li><a href="/products">Produits</a></li>
            <li><a href="/products/new">Nouveau Produit</a></li>
        </ul>
    </nav>
</header>
```

**Action :** Supprimez le second `<header>` qui est une duplication.

---

### Exemple : Tableau des produits
#### Code actuel (dégradé)
```html
<table>
    <thead>
        <tr>
            <th>ID</th>
            <th>Nom</th>
            <th>Prix</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr><td colspan="4"></td></tr> <!-- Ligne inutile -->
        <tr><td colspan="4"></td></tr> <!-- Ligne inutile -->
    </tbody>
</table>
```

#### Code d'origine
```html
<table>
    <thead>
        <tr>
            <th>ID</th>
            <th>Nom</th>
            <th>Prix</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <!-- Les produits dynamiques ici -->
    </tbody>
</table>
```

**Action :** Retirez les lignes `<tr>` inutiles dans `<tbody>`.

