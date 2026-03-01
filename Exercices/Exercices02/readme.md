<p align="Center"><img src="../../includes/logo.png" alt="drawing" width="150"/></p>
<h3 align="Center">2Q2 - Développement Assembleur</h3>

# Exercices 02 - Boucles & cie.

#### 📁 [Structures de projets & consignes à suivre](../../includes/rules.md)

## 4️⃣ Question 01 - ASCII

Créer deux variables x=5 et y=9. Calculer la différence entre y et x et affichez la réponse à l'écran.

```plaintext
4
```

## 🦘 Question 02 - Jump! Jump!

Reproduire ce code C++ en assembleur et le faire rouler avec 85 comme note tout comme 50.

```cpp
int seuil = 60;
int note = 85;
string message ="Vous avez avez obtenu un";
string succes = "succes";
string echec = "echec";
cout << message << " ";
if(note >= seuil) {
   cout << succes;
} else {
   cout << echec;
}
cout << "!";
```

```plaintext
Vous avez avez obtenu un succes!
```

```plaintext
Vous avez avez obtenu un echec!
```

## 🔠 Question 03 - Mr. Alpha Baitte

Écrivez l'alphabet à l'écran comme suit en affichant les caractères un à la fois :

> Interdit d'utiliser l'interruption DOS 09h.

```plaintext
AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz
```

> Utilisez le moins de ligne de code que possible !

## 🚀 Question 04 - Rocketer

Programmez une simulation de lancement de fusée !

```plaintext
9
8
7
6
5
4
3
2
1
DÉCOLLAGE!!!
```

## 🎨 Question 05 - Pablo Picasso del Shawinigan

Recréez simplement ce dessin à l'écran :

```plaintext
**********
*********
********
*******
******
*****
****
***
**
*
```

<hr><p align="Center"><img src="../../includes/end.png" alt="drawing" width="150"/></p>
