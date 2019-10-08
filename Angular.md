==================================
Arrow function => https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions

var materials = [
  'Hydrogen',
  'Helium',
  'Lithium',
  'Beryllium'
];

console.log(materials.map(material => material.length));
// expected output: Array [8, 6, 7, 9]
==================================
RxJS : Reactive programming
debounce : pour ne pas bombarder l'API d'appels obsolètes. Ca clearTimeout à chaque nouveau evenement. Interessant si on va appeler une API de recherche
==================================
TypeScript : utilisé par Angular
Web Component : RFC-Javascript : composante réutilisable pour plusieurs langages/frameworks 

==================================
Component : un
Directive : 
==================================
Karma : tests unitaires
Protractor : tests e2e
==================================
polyfills => rustines/adaptations que le FMW fait pour que le JS marche sur les anciens navigateurs
==================================
Data binding : pour faire communiquer des composants
crochets [] : variables d'entrées
parenthèses() : evenements de sorties
==================================

# Run server
ng server
