### **Rapport de Correction : Travail de Vitiana**

---

#### **Introduction**
Chère Vitiana,

J’ai examiné attentivement ton travail sur la série d’exercices portant sur les bases de Python. Globalement, tu as bien compris les concepts fondamentaux tels que les variables, les types de données, les opérations et les entrées/sorties utilisateur. Cependant, il y a quelques points à améliorer pour rendre ton code encore plus robuste, clair et conforme aux bonnes pratiques de programmation.

Je vais détailler mes commentaires exercice par exercice, en soulignant les forces et les axes d’amélioration. Je te donnerai également des conseils pour progresser davantage.

---

### **Exercice 1 : Déclarer une variable contenant le prénom et l'afficher**

**Code fourni :**
```python
nom="Vivi"
print("Votre nom est :",nom)
```

**Commentaire du professeur :**
- **Force :** 
  - Tu as correctement déclaré une variable `nom` et utilisé la fonction `print` pour afficher son contenu.
  - La syntaxe est impeccable, et le résultat est exact.
  
- **Amélioration :**
  - Ajoute un commentaire au début du programme pour expliquer ce qu’il fait. Cela permettra à toute personne lisant ton code de comprendre immédiatement son objectif.
  
- **Note : 20/20**
  - Excellent travail pour cet exercice !

**Correction suggérée :**
```python
# Programme qui affiche le prénom stocké dans une variable
nom = "Vivi"  # Déclaration de la variable contenant le prénom
print("Votre nom est :", nom)  # Affichage du prénom
```

---

### **Exercice 2 : Créer trois variables (nom, âge, ville) et afficher avec f-string**

**Code fourni :**
```python
nom="Vivi"
age=19
ville="Abidjan"
print(nom,age ,"ans",ville)
```

**Commentaire du professeur :**
- **Force :**
  - Les trois variables sont bien déclarées, et leurs valeurs sont correctes.
  - L’affichage fonctionne correctement.

- **Amélioration :**
  - L'instruction demandait d'utiliser un **f-string** pour formater la chaîne de caractères. Or, tu utilises ici la méthode classique de concaténation avec des virgules. Bien que cela fonctionne, cela ne respecte pas l’énoncé.
  - Il est important de suivre précisément les consignes pour développer une habitude rigoureuse en programmation.

- **Note : 15/20**
  - Pénalité de 5 points pour non-respect de l'utilisation de l'outil f-string.

**Correction suggérée :**
```python
# Déclaration des variables
nom = "Vivi"
age = 19
ville = "Abidjan"

# Affichage avec f-string
print(f"Nom : {nom}, Âge : {age} ans, Ville : {ville}")
```

---

### **Exercice 3 : Demander deux nombres à l'utilisateur et afficher leur somme**

**Code fourni :**
```python
print("Veillez entrer deux nombres")
nbr1=int(input("nombre 1"))
nbr2=int(input("Nombre 2"))
som=nbr1+nbr2
print("La somme est :",som)
```

**Commentaire du professeur :**
- **Force :**
  - Tu as correctement implémenté la demande d’entrée utilisateur avec `input`.
  - La conversion des entrées en entiers (`int`) est bien faite, et la somme est calculée sans erreur.
  
- **Amélioration :**
  - Il y a une petite faute d’orthographe dans "Veillez". Le mot correct est "Veuillez".
  - Ajouter des espaces autour des opérateurs (`=` et `+`) améliore la lisibilité du code.
  
- **Note : 20/20**
  - Bravo pour cet exercice ! Une attention particulière à l'orthographe serait toutefois appréciée.

**Correction suggérée :**
```python
# Demande à l'utilisateur de saisir deux nombres
print("Veuillez entrer deux nombres.")
nbr1 = int(input("Nombre 1 : "))
nbr2 = int(input("Nombre 2 : "))

# Calcul de la somme
som = nbr1 + nbr2

# Affichage du résultat
print("La somme est :", som)
```

---

### **Exercice 4 : Convertir un entier en chaîne de caractères et inversement**

**Code fourni :**
```python
nbr=2300
char="34"
nbrconv=str(nbr)
charconv=int(char)
print(nbr,"et",char)
```

**Commentaire du professeur :**
- **Force :**
  - Les conversions entre entier et chaîne de caractères sont correctement réalisées.
  - Le code fonctionne comme attendu.

- **Amélioration :**
  - L’affichage final pourrait être plus explicite. Actuellement, tu affiches simplement les valeurs initiales (`nbr` et `char`), mais pas les résultats des conversions (`nbrconv` et `charconv`). Cela peut rendre le programme moins clair pour quelqu’un qui lit ton code.
  - Ajouter des commentaires pour expliquer chaque étape serait également bénéfique.

- **Note : 18/20**
  - Pénalité de 2 points pour manque de clarté dans l'affichage des résultats.

**Correction suggérée :**
```python
# Conversion d'un entier en chaîne de caractères
nbr = 2300
nbrconv = str(nbr)

# Conversion d'une chaîne de caractères en entier
char = "34"
charconv = int(char)

# Affichage des résultats
print(f"L'entier {nbr} converti en chaîne de caractères : {nbrconv}")
print(f"La chaîne de caractères '{char}' convertie en entier : {charconv}")
```

---

### **Exercice 5 : Calculer l'aire d'un rectangle**

**Code fourni :**
```python
print("Nous alons calculer l'air d'un rectangle!")
longu=float(input("Entrez la longueur en centimetre"))
large=float(input("Entrez la largeur en centimetre"))
air=longu*large
print("L'air est de",air,"cm")
```

**Commentaire du professeur :**
- **Force :**
  - Le calcul de l’aire est correct.
  - Les conversions en flottants (`float`) sont bien effectuées pour gérer des dimensions décimales.

- **Amélioration :**
  - Il y a deux fautes d’orthographe :
    - "alons" → "allons".
    - "air" → "aire".
  - L’unité finale est incorrecte : "cm" devrait être "cm²" pour indiquer une surface.
  - Ajouter des espaces autour des opérateurs (`=` et `*`) améliore la lisibilité du code.

- **Note : 17/20**
  - Pénalité de 3 points pour les fautes d’orthographe et l’erreur d’unité.

**Correction suggérée :**
```python
# Calcul de l'aire d'un rectangle
print("Nous allons calculer l'aire d'un rectangle !")

# Saisie des dimensions
longu = float(input("Entrez la longueur en centimètres : "))
large = float(input("Entrez la largeur en centimètres : "))

# Calcul de l'aire
aire = longu * large

# Affichage du résultat avec l'unité correcte
print(f"L'aire est de {aire} cm².")
```

---

### **Conclusion**

#### **Répartition des notes :**
1. Exercice 1 : **20/20**
2. Exercice 2 : **15/20**
3. Exercice 3 : **20/20**
4. Exercice 4 : **18/20**
5. Exercice 5 : **17/20**

#### **Note globale : 90/100**

---

#### **Remarques générales :**
- Ton travail montre une bonne compréhension des bases de Python. Continue ainsi !
- Pour progresser davantage :
  - Sois attentive aux consignes exactes des exercices.
  - Améliore la lisibilité de ton code avec des espaces et des commentaires.
  - Révise l’orthographe et les conventions d’écriture (par exemple, les unités).

En intégrant ces ajustements, tu atteindras facilement un niveau parfait. Continue à travailler avec cette même motivation, et n’hésite pas à poser des questions si besoin.

Bravo pour tes efforts, Vitiana ! 🌟