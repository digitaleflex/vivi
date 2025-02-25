### **Rapport de Correction : Travail de Vitiana (Série 2)**

---

#### **Introduction**
Chère Vitiana,

J’ai examiné attentivement ton travail sur la série d’exercices portant sur les structures conditionnelles (`if`, `elif`, `else`). Globalement, tu as bien compris le fonctionnement des conditions en Python et as fourni des solutions correctes pour la plupart des exercices. Cependant, il y a quelques points à améliorer pour rendre ton code encore plus robuste, clair et conforme aux bonnes pratiques.

Je vais détailler mes commentaires exercice par exercice, en soulignant les forces et les axes d’amélioration. Je te donnerai également des conseils pour progresser davantage.

---

### **Exercice 1 : Vérifier si un nombre est pair ou impair**

**Code fourni :**
```python
nbr = int(input("Veillez entrer un nombre : "))
reste = nbr % 2
if reste == 0:
    print("Ce nombre est pair !")
else:
    print("Ce nombre est impair !")
```

**Commentaire du professeur :**
- **Force :**
  - Le code fonctionne parfaitement.
  - Tu utilises correctement l’opérateur modulo (`%`) pour vérifier si le nombre est divisible par 2.
  
- **Amélioration :**
  - Corrige l'orthographe de "Veillez" → "Veuillez".
  - Ajoute un commentaire au début du programme pour expliquer son objectif.

- **Note : 20/20**
  - Excellent travail pour cet exercice !

**Correction suggérée :**
```python
# Programme qui vérifie si un nombre est pair ou impair
nbr = int(input("Veuillez entrer un nombre : "))
reste = nbr % 2

if reste == 0:
    print("Ce nombre est pair !")
else:
    print("Ce nombre est impair !")
```

---

### **Exercice 2 : Vérifier si une personne est mineure ou majeure**

**Code fourni :**
```python
age = int(input("Quel est votre age ? : "))
if 0 < age < 18:
    print("Vous etes mineur !")
elif age >= 18:
    print("Vous etes majeur !")
```

**Commentaire du professeur :**
- **Force :**
  - La logique est correcte, et le code fonctionne comme attendu.
  - L’utilisation de `elif` est appropriée pour gérer les deux cas possibles.

- **Amélioration :**
  - Il manque un cas pour gérer les valeurs incorrectes d’âge (par exemple, des nombres négatifs ou des entrées non valides). Bien que ce ne soit pas explicitement demandé dans l’énoncé, cela rendrait ton programme plus robuste.
  - Corrige l'orthographe de "etes" → "êtes".

- **Note : 18/20**
  - Pénalité de 2 points pour l’absence de gestion des cas d’erreur.

**Correction suggérée :**
```python
# Programme qui vérifie si une personne est mineure ou majeure
age = int(input("Quel est votre âge ? : "))

if age < 0:
    print("Erreur : l'âge ne peut pas être négatif.")
elif age < 18:
    print("Vous êtes mineur !")
else:
    print("Vous êtes majeur !")
```

---

### **Exercice 3 : Vérifier si un nombre est positif, négatif ou nul**

**Code fourni :**
```python
nbr = float(input("Veillez entrer un nombre : "))
if nbr > 0:
    print("Ce nombre est positif")
elif nbr < 0:
    print("Ce nomrbre est negatif")
elif nbr == 0:
    print("Ce nombre est nul")
```

**Commentaire du professeur :**
- **Force :**
  - La logique est correcte, et le code fonctionne comme attendu.
  - Tu utilises correctement les comparaisons (`>`, `<`, `==`).

- **Amélioration :**
  - Corrige l'orthographe de "nomrbre" → "nombre".
  - Ajoute des espaces autour des opérateurs (`>` et `<`) pour améliorer la lisibilité.
  - Ajoute un commentaire pour expliquer le but du programme.

- **Note : 19/20**
  - Pénalité de 1 point pour l’orthographe.

**Correction suggérée :**
```python
# Programme qui vérifie si un nombre est positif, négatif ou nul
nbr = float(input("Veuillez entrer un nombre : "))

if nbr > 0:
    print("Ce nombre est positif.")
elif nbr < 0:
    print("Ce nombre est négatif.")
else:
    print("Ce nombre est nul.")
```

---

### **Exercice 4 : Simuler un mot de passe**

**Code fourni :**
```python
Mdp = "asfhdffk3456"
mdp_user = str(input("Veillez entrer un mot de passe : "))
if mdp_user == Mdp:
    print("Ce mot de passe existe deja !")
else:
    print("Mot de passe enregistre !")
```

**Commentaire du professeur :**
- **Force :**
  - La logique est correcte, et le code fonctionne comme attendu.
  - Tu compares correctement le mot de passe entré par l’utilisateur avec la valeur prédéfinie.

- **Amélioration :**
  - Corrige l'orthographe de "Veillez" → "Veuillez".
  - Les messages affichés peuvent être améliorés pour être plus clairs :
    - "Ce mot de passe existe déjà !" → "Mot de passe correct."
    - "Mot de passe enregistre !" → "Mot de passe incorrect."
  - Ajoute un commentaire pour expliquer le but du programme.

- **Note : 18/20**
  - Pénalité de 2 points pour l’orthographe et la clarté des messages.

**Correction suggérée :**
```python
# Programme qui simule une vérification de mot de passe
Mdp = "asfhdffk3456"
mdp_user = input("Veuillez entrer un mot de passe : ")

if mdp_user == Mdp:
    print("Mot de passe correct.")
else:
    print("Mot de passe incorrect.")
```

---

### **Exercice 5 : Vérifier si un nombre est un multiple de 3 ou de 5**

**Code fourni :**
```python
nbr = int(input("Veillez entrer un nombre : "))
if nbr % 5 == 0:
    print("Ce nombre est un multiple de 5")
elif nbr % 3 == 0:
    print("Ce nombre est un multiple de 3")
else:
    print("Ce nombre n'est ni un multiple 5, ni un multiple de 3")
```

**Commentaire du professeur :**
- **Force :**
  - La logique est correcte, et le code fonctionne comme attendu.
  - Tu utilises correctement les conditions pour vérifier les multiples.

- **Amélioration :**
  - Corrige l'orthographe de "Veillez" → "Veuillez".
  - Ajoute des espaces autour des opérateurs (`%`) pour améliorer la lisibilité.
  - Gère le cas où le nombre est à la fois un multiple de 3 **et** de 5 (par exemple, 15). Actuellement, ton programme ne prendra en compte que le premier test (`if nbr % 5 == 0`).

- **Note : 17/20**
  - Pénalité de 3 points pour l’orthographe et la gestion incomplète des multiples.

**Correction suggérée :**
```python
# Programme qui vérifie si un nombre est un multiple de 3 ou de 5
nbr = int(input("Veuillez entrer un nombre : "))

if nbr % 3 == 0 and nbr % 5 == 0:
    print("Ce nombre est un multiple de 3 et de 5.")
elif nbr % 5 == 0:
    print("Ce nombre est un multiple de 5.")
elif nbr % 3 == 0:
    print("Ce nombre est un multiple de 3.")
else:
    print("Ce nombre n'est ni un multiple de 3, ni un multiple de 5.")
```

---

### **Conclusion**

#### **Répartition des notes :**
1. Exercice 1 : **20/20**
2. Exercice 2 : **18/20**
3. Exercice 3 : **19/20**
4. Exercice 4 : **18/20**
5. Exercice 5 : **17/20**

#### **Note globale : 92/100**

---

#### **Remarques générales :**
- Ton travail montre une bonne compréhension des structures conditionnelles en Python. Continue ainsi !
- Pour progresser davantage :
  - Sois attentive aux consignes exactes des exercices.
  - Améliore la lisibilité de ton code avec des espaces et des commentaires.
  - Révise l’orthographe et les conventions d’écriture.
  - Anticipe les cas d’erreur pour rendre tes programmes plus robustes.

En intégrant ces ajustements, tu atteindras facilement un niveau parfait. Continue à travailler avec cette même motivation, et n’hésite pas à poser des questions si besoin.

Bravo pour tes efforts, Vitiana ! 🌟