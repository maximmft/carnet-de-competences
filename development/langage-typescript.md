# TypeScript

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

### L'intérêt de TypeScript dans l'IDE ✅ 

**Explication :**  
TypeScript apporte des **types statiques** au JavaScript, ce qui permet à l'IDE de :  
- Détecter les erreurs avant l'exécution (exemple : passer une string au lieu d’un number).  
- Fournir des suggestions (autocomplétion) basées sur les types.  
- Faciliter la navigation dans le code (aller à la définition d’une fonction ou d’un type).

**Exemple :**
```typescript
function add(a: number, b: number): number {
  return a + b;
}

add(2, "3"); // Erreur signalée par l'IDE avant l'exécution
```

**Avantages :**
- Réduction des bugs liés aux types.
- Productivité améliorée grâce à l’autocomplétion.
- Maintenance du code facilitée.

---

### Les types de base ✅ 

**Explication :**  
Les types de base permettent de définir clairement le type de données attendu :

- string : Chaîne de caractères  
- number : Nombre (entier ou décimal)  
- boolean : Vrai ou Faux  
- array : Tableau  
- any : N'importe quel type (à éviter)  
- void : Pas de retour (pour les fonctions)  
- null/undefined : Valeurs nulles ou non définies  

**Exemple :**
```typescript
let name: string = "Maxime";
let age: number = 28;
let isDeveloper: boolean = true;
let hobbies: string[] = ["coding", "reading"];
let user: [string, number] = ["Maxime", 28]; // Tuple
```

---

### Comment et pourquoi étendre une interface ✅ 

**Explication :**  
L'extension d'une interface permet de **réutiliser** des définitions existantes tout en ajoutant de nouvelles propriétés. Cela favorise la modularité et évite la duplication.

**Exemple :**
```typescript
interface User {
  id: number;
  name: string;
  email: string;
}

interface Admin extends User {
  permissions: string[];
}

const admin: Admin = {
  id: 1,
  name: "Maxime",
  email: "maxime@example.com",
  permissions: ["manage-users", "delete-posts"]
};
```

**Avantages :**
- Réduction de la duplication de code.
- Cohérence dans les structures de données.
- Simplification des évolutions : ajouter une propriété à `User` affecte automatiquement `Admin`.

---

### Les classes et les decorators ✅ 

#### Classes  
TypeScript ajoute des fonctionnalités orientées objet à JavaScript. Les classes permettent de créer des objets avec des propriétés et des méthodes, facilitant la réutilisation et la modularité.

**Exemple :**
```typescript
class User {
  id: number;
  name: string;

  constructor(id: number, name: string) {
    this.id = id;
    this.name = name;
  }

  greet(): string {
    return `Hello, ${this.name}!`;
  }
}

const user = new User(1, "Maxime");
console.log(user.greet()); // "Hello, Maxime!"
```

#### Decorators  
Les decorators sont des fonctions spéciales qui modifient le comportement des classes, méthodes, propriétés ou paramètres. Ils sont utilisés dans des frameworks comme **NestJS** ou **Angular**.

**Exemple :**
```typescript
function Log(target: any, key: string) {
  console.log(`La propriété "${key}" a été décorée.`);
}

class Product {
  @Log
  name: string;

  constructor(name: string) {
    this.name = name;
  }
}

const product = new Product("Laptop");
// Console : "La propriété 'name' a été décorée."
```

---

## 💻 J'utilise

### Un exemple personnel commenté ✔️

```
export type AdCardProps = {
	id:number
	title: string;
	picture: string;
	price: number;
};
```

### Utilisation dans un projet ✔️

[https://github.com/maximmft/dark-corner/blob/main/frontend/src/components/AdCard.tsx](...)

Description : Ce projet est un miniprojet reprenant le concept du Bon Coin

### Utilisation en production si applicable❌

[lien du projet](...)

Description :

### Utilisation en environement professionnel ✔️

Description : J'utilise typescript dans mon alternance

## 🌐 J'utilise des ressources

### Titre

- lien
- description

## 🚧 Je franchis les obstacles

### Point de blocage ✔️

Description: Blocage sur les décorateurs

Plan d'action : (à valider par le formateur)

- action 1: Revoir les concepts ❌ / ✔️
- action 2: Utiliser un décorateur dans un projet ❌ / ✔️
- ...

Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌  
- J'ai fait une [présentation](...) ❌  
