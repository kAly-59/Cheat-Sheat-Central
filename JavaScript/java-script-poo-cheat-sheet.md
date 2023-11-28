# Concepts fondamentaux de la POO en JavaScript :

- **Objets** : Instances de classes, contenant des attributs et des méthodes.
  ```javascript
  // Définition d'une classe (fonction constructeur)
  function Voiture(marque, couleur) {
      this.marque = marque; // Attribut
      this.couleur = couleur; // Attribut
  
      this.demarrer = function() { // Méthode
          return `La voiture de marque ${this.marque} démarre.`;
      };
  }
  
  // Création d'objets
  const voiture1 = new Voiture("Toyota", "rouge");
  const voiture2 = new Voiture("BMW", "noir");
  
  console.log(voiture1.demarrer()); // Appel d'une méthode sur un objet
  console.log(voiture2.demarrer());
  ```

- **Attributs** : Variables définissant l'état des objets.
  ```javascript
  function Chien(nom, age) {
      this.nom = nom; // Attribut
      this.age = age; // Attribut
  }
  
  const chien1 = new Chien("Rex", 3);
  console.log(chien1.nom); // Accès à l'attribut
  console.log(chien1.age);
  ```

- **Méthodes** : Fonctions définies dans une classe agissant sur les attributs.
  ```javascript
  function Calculatrice() {}
  
  Calculatrice.prototype.addition = function(a, b) { // Méthode
      return a + b;
  };
  
  Calculatrice.prototype.soustraction = function(a, b) { // Méthode
      return a - b;
  };
  
  const calc = new Calculatrice();
  console.log(calc.addition(5, 3)); // Appel d'une méthode
  console.log(calc.soustraction(10, 4));
  ```

- **Classes** : Modèles pour créer des objets avec attributs et méthodes. *(Remarque : JavaScript introduit la syntaxe de classe dans ES6, bien que cela soit une syntaxe de sucre syntaxique et que JavaScript reste basé sur des prototypes.)*
  ```javascript
  class Personne {
      constructor(nom, age) {
          this.nom = nom;
          this.age = age;
      }
  }
  
  const personne1 = new Personne("Alice", 25);
  const personne2 = new Personne("Bob", 30);
  ```

- **Constructeurs** : Méthodes spéciales pour initialiser de nouveaux objets.
  ```javascript
  function Point(x, y) {
      this.x = x;
      this.y = y;
  }
  
  const point1 = new Point(3, 4); // Création d'un objet
  ```

- **Héritage** : Capacité pour une classe de bénéficier des caractéristiques d'une autre.
  ```javascript
  function Animal() {}
  
  Animal.prototype.manger = function() {
      return "L'animal mange.";
  };
  
  function Chien() {}
  Chien.prototype = Object.create(Animal.prototype); // Héritage
  
  Chien.prototype.aboyer = function() {
      return "Le chien aboie.";
  };
  
  const chien = new Chien();
  console.log(chien.manger()); // Accès à une méthode héritée
  console.log(chien.aboyer());
  ```

- **Encapsulation** : Regroupement de données et méthodes dans une entité.
  ```javascript
  function CompteBancaire(solde) {
      let soldeCourant = solde; // Attribut encapsulé
  
      this.getSolde = function() {
          return soldeCourant;
      };
  
      this.deposer = function(montant) {
          soldeCourant += montant;
      };
  }
  
  const compte = new CompteBancaire(1000);
  console.log(compte.getSolde()); // Accès à l'attribut encapsulé
  compte.deposer(500);
  ```

- **Abstraction** : Représentation des caractéristiques essentielles sans détails d'implémentation.
  ```javascript
  class Forme {
      aire() { // Méthode abstraite
          throw new Error("Méthode aire() non implémentée.");
      }
  }
  
  class Carre extends Forme {
      constructor(cote) {
          super();
          this.cote = cote;
      }
  
      aire() {
          return this.cote ** 2;
      }
  }
  
  const carre = new Carre(5);
  console.log(carre.aire());
  ```

- **Interfaces** : Définition de méthodes sans implémentation à implémenter par d'autres classes.
  ```javascript
  class Carre {
      constructor(cote) {
          this.cote = cote;
      }
  
      aire() {
          return this.cote ** 2;
      }
  }
  
  const carre = new Carre(5);
  console.log(carre.aire());
  ```

- **Polymorphisme** : Traitement uniforme d'objets de classes différentes possédant des méthodes similaires.
  ```javascript
  class Animal {
      son() {}
  }
  
  class Chien extends Animal {
      son() {
          return "Woof!";
      }
  }
  
  class Chat extends Animal {
      son() {
          return "Meow!";
      }
  }
  
  const animaux = [new Chien(), new Chat()];
  animaux.forEach(animal => {
      console.log(animal.son());
  });
  ```
