# hashcode

## Recherche Opérationnelle

J'ai fait des fichiers templates pour deux approches

- Pulp :
  - Programmation linéaire (wrapper pour les solvers COIN-OR ou Gurobi)
  - Positif : en python, rapide si ~10^7 variables
  - Négatif : contraintes et expressions sont des CL de variables

- Localsolver :
  - Solver généraliste
  - Positif : contraintes et expressions arbitraires
  - Négatif : en C++, peu être lent si beaucoup d'expressions (10^8)
  - Commande pour compiler (remplace "model.cc" par nom du fichier source) :
  
  ```
  g++ model.cc -ls -llocalsolver -lpthread -o model
  ```

Pour les utiliser il faut SSH sur mon PC parce qu'ils ont besoin de licences
Je vous filerai adresse et clés jeudi