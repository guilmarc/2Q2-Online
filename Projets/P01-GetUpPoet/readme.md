<p align="Center"><img src="../../includes/logo.png" alt="drawing" width="100"/></p>
<h4 align="Center">2Q2 - Développement Assembleur</h3>

<h1 align="Center">⬆️ Get Up! Poet! ⬆️</h1>
<p align="Center"><img src="./includes/logo.png" alt="drawing" width="550"/></p>


## ✅ [Consignes à suivre](../../includes/rules-project.md)

# La phobie des majuscules

Didier Laplume est un poète parisien célèbre pour ses œuvres empreintes d'une touche d'humanisme.  Il publie des centaines de poèmes tout au long de l'année.

Didier a une drôle de phobie, il est terrorisé par les lettres majuscules.  Il écrit toutes ses œuvres avec des lettres minuscules.

Son éditeur est essoufflé de devoir modifier tous les poèmes de Didier et vous demande de créer un programme qui prendra ses œuvres originales et placera les majuscules en début de chacunes des phrases.

### Oeuvre originale de Didier :
```plaintext
je garde un espoir simple.
dans un geste discret.
une main tendue.
un sourire sans raison.

je vois des gens qui réparent.
qui s’excusent.
qui apprennent.
qui se relèvent après l’erreur.
et qui choisissent encore la bonté.

l’humanité vacille parfois.
mais elle avance.
a petits pas.
avec du courage ordinaire.
et je crois que demain peut être meilleur.
```
### Oeuvre publiés par son éditeur :
```plaintext
Je garde un espoir simple.
Dans un geste discret.
Une main tendue.
Un sourire sans raison.

Je vois des gens qui réparent.
Qui s’excusent.
Qui apprennent.
Qui se relèvent après l’erreur.
Et qui choisissent encore la bonté.

L’humanité vacille parfois.
Mais elle avance.
A petits pas.
Avec du courage ordinaire.
Et je crois que demain peut être meilleur.
```
# Spécifications technique
1. Créer une variable `source` qui contienda l'oeuvre source de Didier Laplume, nuancée de sa phobie des lettres majuscules.
2. Créez une variable `poem` qui contiendra le poème final à publier.
3. Transformez l'oeuvre source selon la demande.
4. Assurez-vous que le poème final soit présent dans la variable `poem`.
5. Afficher directement le poème final à l'écran.

> RAPPELS : 
> 1. `string` est l'équivalent de `char[]`.
> 2. Un `boolean` est souvent utilisé afin de mémoriser si une action doit être exécutée, exemple (`hasToGetUp`).
> 3. Avoir du plaisir à transcoder cotre *pseudocode* c++ en assembleur n'est pas défendu !



## Information complémentaire
Étant donné que nous n'avons pas encore appris à lire à partir d'un fichier, nous utiliserons la déclaration de chaîne de caractères multilignes afin d'obtenir l'oeuvre source.  Voici comment effectuer une déclaration multiligne :
### En C++ :
```cpp
string source =
  "je garde un espoir simple.\n"
  "dans un geste discret.\n"
  [...]
  "et je crois que demain peut être meilleur.\0";
```
### En ASM8086 :
```assembly
source db "Je garde un espoir simple.",0Dh,0Ah
       db "Dans un geste discret.",0Dh,0Ah
       [...]
       db "Et je crois que demain peut etre meilleur.$"
```

> ATTENTION : `\0` représente le caractère de fin de chaîne en C++.  Il est équivalent au caractère `$` en ASM8086.

<hr><p align="Center"><img src="../../includes/end.png" alt="drawing" width="150"/></p>
