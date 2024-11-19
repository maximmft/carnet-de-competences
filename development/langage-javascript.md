# Langage Javascript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- les `structures` de base du langage ✔️  
    Lors de mon DWWM j'ai appris les structures fondamentales en JavaScript, telles que les variables (let et const), les structures conditionnelles (if, else,         switch), les boucles (for, while, forEach), ainsi que les fonctions (déclaratives, fléchées et anonymes).
  
- les normes `ecmascript` ✔️  
      Je sais utiliser la déstructuration pour extraire facilement des données d’objets ou de tableaux, les modules (import/export) pour structurer mon code, ou          les classes pour créer des objets réutilisables. J’utilise aussi les fonctions fléchées pour simplifier mon code
  
- l'utilisation de l'`asynchrone` ✔️  
      J’utilise les Promises pour gérer des retours de données. Avec les mots-clés async et await, je simplifie l’écriture du code asynchrone, en le rendant plus         lisible et proche du code synchrone. Je les utilise pour appeler des API via fetch.

- les spécifités du mot-clef `this` ✔️  
      Dans une fonction classique, this fait référence à l’objet qui appelle la fonction, tandis que dans une fonction fléchée, il hérite de son contexte parent.

## 💻 Je code en Javascript

### Un exemple de code commenté ✔️

```javascript
//Je parcours mes catégories en les affichant avec leur photo, nom et détails
{cat.map((category) => ( 
        <div key={category.Id_category_list} className="category-container">
          <div
            onClick={() => handleCategories(category)}
            onKeyDown={handleCategories}
            role="presentation"
            style={{ backgroundImage: `url(${category.picture})` }}
            className="category-image"
          >
            <h1 className="category-title">{category.title}</h1>
            <h2 className="order-title">{category.details}</h2>
          </div>
        </div>
      ))}
```

### Utilisation dans un projet ✔️

[https://github.com/WildCodeSchool-2024-02/JS-Paris-BrainWaves-P3-Gems/](...)

Description : Ce projet est mon projet de validation de DWWM, un site de vente de bijous entre particulier

### J'ai utilisé ce langage en production ✔️

[https://github.com/WildCodeSchool-2024-02/JS-Paris-BrainWaves-P3-Gems/](...)

[https://gems-gems.fr/](...)

Description : Ce projet est mon projet de validation de DWWM, un site de vente de bijous entre particulier

### J'ai utilisé ce langage en environement professionnel ✔️

Description : Lors de mon alternance je code sur React.js sur le projet qui est une plateforme de mise en relation entre Spa et hôtels de luxe

## 🌐 J'utilise des ressources

### Titre

- lien
- description

## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

Plan d'action : (à valider par le formateur)

- action 1 ❌ / ✔️
- action 2 ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ 
- J'ai fait une [présentation](...) ❌ 

