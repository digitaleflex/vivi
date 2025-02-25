### **Rapport de Correction : Travail de Vitiana (Série 3)**

---

#### **Introduction**
Chère Vitiana,

J’ai examiné attentivement ton travail sur la série d’exercices portant sur les boucles (`for` et `while`). Globalement, tu as bien compris le fonctionnement des boucles en Python et as fourni des solutions correctes pour la plupart des exercices. Cependant, il y a quelques points à améliorer pour rendre ton code encore plus robuste, clair et conforme aux bonnes pratiques.

Je vais détailler mes commentaires exercice par exercice, en soulignant les forces et les axes d’amélioration. Je te donnerai également des conseils pour progresser davantage.

---

### **Exercice 1 : Afficher les nombres de 1 à 10 avec une boucle `for`**

**Code fourni :**
```python
for i in range(1, 11):
    print(i)
```

**Commentaire du professeur :**
- **Force :**
  - Le code fonctionne parfaitement.
  - Tu utilises correctement la fonction `range()` pour itérer de 1 à 10 inclus.

- **Amélioration :**
  - Ajoute un commentaire au début du programme pour expliquer son objectif.

- **Note : 20/20**
  - Excellent travail pour cet exercice !

**Correction suggérée :**
```python
# Programme qui affiche les nombres de 1 à 10 avec une boucle for
for i in range(1, 11):
    print(i)
```

---

### **Exercice 2 : Afficher les nombres pairs entre 1 et 20 avec une boucle `while`**

**Code fourni :**
```python
for i in range(1, 21):
    while i % 2 == 0:
        print(i)
        i += 1
```

**Commentaire du professeur :**
- **Problème principal :**
  - L’utilisation combinée de `for` et `while` est incorrecte ici. La boucle `while` n’est pas nécessaire dans ce contexte car la boucle `for` suffit à parcourir les nombres de 1 à 20.
  - La variable `i` est incrémentée deux fois : une fois automatiquement par `for` et une autre fois manuellement dans le `while`. Cela provoque une erreur logique.

- **Solution :**
  - Utilise uniquement une boucle `while` ou une boucle `for` pour résoudre l’exercice.

- **Note : 10/20**
  - Pénalité de 10 points pour l’erreur logique et l’utilisation incorrecte des boucles.

**Correction suggérée (avec `while`) :**
```python
# Programme qui affiche les nombres pairs entre 1 et 20 avec une boucle while
i = 1
while i <= 20:
    if i % 2 == 0:
        print(i)
    i += 1
```

**Correction alternative (avec `for`) :**
```python
# Programme qui affiche les nombres pairs entre 1 et 20 avec une boucle for
for i in range(1, 21):
    if i % 2 == 0:
        print(i)
```

---

### **Exercice 3 : Faire deviner un nombre aléatoire entre 1 et 10 avec `while`**

**Code fourni :**
```python
print("Devinez le nombre secret!")
nbr_user = int(input())
while nbr_user != 39:
    nbr_user = int(input("Essaye encore !"))
if nbr_user == 39:
    print("Bien jouer !")
```

**Commentaire du professeur :**
- **Force :**
  - La logique est correcte, et le code fonctionne comme attendu.
  - Tu utilises correctement la boucle `while` pour répéter la demande tant que l’utilisateur ne devine pas le bon nombre.

- **Amélioration :**
  - Le nombre secret est fixé à 39, mais l’énoncé demandait un nombre aléatoire entre 1 et 10. Il faut utiliser le module `random` pour générer un nombre aléatoire.
  - Corrige l'orthographe de "jouer" → "joué".

- **Note : 15/20**
  - Pénalité de 5 points pour non-respect de l’énoncé (nombre aléatoire).

**Correction suggérée :**
```python
import random

# Génération du nombre secret aléatoire entre 1 et 10
nombre_secret = random.randint(1, 10)

print("Devinez le nombre secret (entre 1 et 10) !")
nbr_user = int(input())

while nbr_user != nombre_secret:
    nbr_user = int(input("Essaie encore ! "))

print("Bien joué !")
```

---

### **Exercice 4 : Afficher la table de multiplication d’un nombre entré par l’utilisateur**

**Code fourni :**
```python
print("TABLE DE MULTIPLICATION")
nbr_table = int(input("Quelle table souhaitez vous afficher? "))
for i in range(0, 11):
    print(nbr_table, "x", i, "=", nbr_table * i)
```

**Commentaire du professeur :**
- **Force :**
  - Le code fonctionne correctement.
  - Tu utilises correctement la boucle `for` pour afficher la table de multiplication.

- **Amélioration :**
  - Ajoute un espace après la question pour améliorer la lisibilité de l’invite utilisateur.
  - Utilise un f-string pour formater l’affichage de manière plus élégante.

- **Note : 19/20**
  - Pénalité de 1 point pour l’absence d’espaces autour des opérateurs.

**Correction suggérée :**
```python
# Programme qui affiche la table de multiplication d'un nombre donné
print("TABLE DE MULTIPLICATION")
nbr_table = int(input("Quelle table souhaitez-vous afficher ? "))

for i in range(0, 11):
    print(f"{nbr_table} x {i} = {nbr_table * i}")
```

---

### **Exercice 5 : Calculer la somme des nombres de 1 à n avec `for`**

**Code fourni :**
```python
nbr_som = 0
nbr = int(input("Vous voulez faire la somme des nombres jusqu'à combien ? : "))
for i in range(1, nbr + 1):
    nbr_som += i
print("La somme des nombres de 1 à", nbr, "est :", nbr_som)
```

**Commentaire du professeur :**
- **Force :**
  - Le code fonctionne parfaitement.
  - Tu utilises correctement la boucle `for` pour calculer la somme.

- **Amélioration :**
  - Utilise un f-string pour formater l’affichage final de manière plus élégante.

- **Note : 20/20**
  - Excellent travail pour cet exercice !

**Correction suggérée :**
```python
# Programme qui calcule la somme des nombres de 1 à n
nbr_som = 0
nbr = int(input("Vous voulez faire la somme des nombres jusqu'à combien ? : "))

for i in range(1, nbr + 1):
    nbr_som += i

print(f"La somme des nombres de 1 à {nbr} est : {nbr_som}")
```

---

### **Conclusion**

#### **Répartition des notes :**
1. Exercice 1 : **20/20**
2. Exercice 2 : **10/20**
3. Exercice 3 : **15/20**
4. Exercice 4 : **19/20**
5. Exercice 5 : **20/20**

#### **Note globale : 86/100**

---

#### **Remarques générales :**
- Ton travail montre une bonne compréhension des boucles en Python. Continue ainsi !
- Pour progresser davantage :
  - Sois attentive aux consignes exactes des exercices (par exemple, l’utilisation de nombres aléatoires).
  - Améliore la lisibilité de ton code avec des espaces et des commentaires.
  - Révise l’orthographe et les conventions d’écriture.

En intégrant ces ajustements, tu atteindras facilement un niveau parfait. Continue à travailler avec cette même motivation, et n’hésite pas à poser des questions si besoin.

Bravo pour tes efforts, Vitiana ! 🌟