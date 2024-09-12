import 'dart:collection';

void main() {

  List<int> nombres = [1, 2, 3, 4, 5,6,7,8,9,10]; 
  
  
  nombres.add(15);
  nombres.removeAt(0);
  nombres.removeLast();
    
  int sum = 0;
  for(int nombre in nombres){
    sum+=nombre;
  }
  print(sum);

  // Trier la liste en ordre décroissant
  nombres.sort((a, b) => b.compareTo(a));

  // Obtenir une sous-liste
  List<int> obteList = nombres.sublist(1, 9); // Par exemple, de l'index 1 à 3 (4 exclu)

  print(nombres); // Affiche la liste triée
  print(obteList); // Affiche la sous-liste
Set<String>villes = {"Paris", "Londres","New York","Berlin","Tokyo",""};
  villes.add("Paris");
  villes.add("Rio de Janeiro");
print(villes);
    villes.remove("Londres");
print(villes);
  
List<String>alph =villes.toList();
  alph.sort();
  villes=alph.toSet();
print(villes);  

  

if (villes.contains("Tokyo")) {
  print("Tokyo existe!");
}

//   3
  Map<String, int> nomNotes = {'Alice': 30, 'Bob': 25, 'Charlie': 35};
//   ajout 
nomNotes['Julie'] = 40;
nomNotes['Alain'] = 50;
nomNotes['Pierre'] = 80;
nomNotes['Albertine'] = 20;
nomNotes['Elise'] = 30;
print(nomNotes);
  
//   supprimer bob
  nomNotes.remove("Bob");
  print(nomNotes);
  
//   ajouter charlie
  nomNotes['Charlie'] = 18;
    print(nomNotes);

int somme = 0;

// Utilisation d'une boucle for pour parcourir les valeurs du Map
for (int note in nomNotes.values) {
  somme += note;
}

// Calculer la moyenne
double moyenne = somme / nomNotes.length;

print("La moyenne des notes des étudiants est : $moyenne");

 


  // Créer une Queue vide
  Queue<String> fileAttente = Queue();

  // Ajouter 5 personnes à la file d'attente
  fileAttente.addAll(["Alice", "Bob", "Charlie", "David", "Eva"]);

  // Supprimer deux personnes de la file d'attente (leur tour est passé)
  fileAttente.removeFirst(); // Alice part
  fileAttente.removeFirst(); // Bob part

  // Ajouter deux nouvelles personnes à la file
  fileAttente.addAll(["Frank", "Grace"]);

  // Afficher la personne en tête de la file
  print("La personne en tête de la file est : ${fileAttente.first}");

  // Afficher la file complète après les opérations
  print("La file complète est : $fileAttente");
}










