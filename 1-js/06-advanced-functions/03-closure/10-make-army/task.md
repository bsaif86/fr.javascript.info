importance: 5

---

# Armée de fonctions

Le code suivant crée un tableau de `shooters`.

Chaque fonction est censée sortir son numéro. Mais quelque chose ne va pas …

```js run
function makeArmy() {
  let shooters = [];

  let i = 0;
  while (i < 10) {
<<<<<<< HEAD
    let shooter = function() { // shooter function
      alert( i ); // devrait afficher son numéro
=======
    let shooter = function() { // create a shooter function,
      alert( i ); // that should show its number
>>>>>>> 181cc781ab6c55fe8c43887a0c060db7f93fb0ca
    };
    shooters.push(shooter); // and add it to the array
    i++;
  }

  // ...and return the array of shooters
  return shooters;
}

let army = makeArmy();

<<<<<<< HEAD
army[0](); // the shooter numéro 0 affiche 10
army[5](); // et le numéro 5 affiche aussi 10...
// ... tous les shooters affichent 10 au lieu de 0, 1, 2, 3 …
```

Pourquoi tous les shooters affichent la même valeur ? Corrigez le code pour qu’ils fonctionnent comme prévu.
=======
*!*
// all shooters show 10 instead of their numbers 0, 1, 2, 3...
army[0](); // 10 from the shooter number 0
army[1](); // 10 from the shooter number 1
army[2](); // 10 ...and so on.
*/!*
```

Why do all of the shooters show the same value? 

Fix the code so that they work as intended.

>>>>>>> 181cc781ab6c55fe8c43887a0c060db7f93fb0ca
