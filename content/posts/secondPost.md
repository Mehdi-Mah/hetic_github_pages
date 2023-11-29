+++
title = 'Python'
date = 2023-11-27T13:57:31+01:00
draft = false
summary = "Pourquoi Python ? J'ai décidé de parler de python, comme à l'heure où j'écris ce post je découvre ce langage..."
+++

![Logo Python](https://www.python.org/static/community_logos/python-logo-master-v3-TM.png)
# Mes début en Python
***J'ai décidé de parler des bases que j'ai appris en Python, comme à l'heure où j'écris ce post je découvre ce langage.***
## C'est quoi Python ?

Python est un langage de programmation interprété et de haut niveau.
C'est un langage polyvalent, avec une syntaxe claire et concise.


## Les notions de bases appris

On a également eu un cours de data-science le Mardi 28 Novembre, dans lequel nous avons utilisé Python. J'ai donc pu approfondir les notions de bases de Python lors de ce cours.

### Les déclarations de variables

Pour définir des variables, comme en PHP ou en JS, il n'y avait pas besoin de définir de type pour les variables (contrairement au C par exemple).
Pour les int, string et float:

```python
valueInt = 5
valueString = "ma value"
valueFloat = 3.5
```

Ensuite j'ai pu voir que pour *concaténer* différentes valeurs il fallait sépérarer mes différentes valeurs avec **l'opérateur +**.

### Les conditions et les boucles

Alors pour les conditions (if, else, elseif) la syntaxe était un peu différente des langages que j'utilisais.

```python
if condition1:
    # Code à exécuter si la condition1 est vraie
elif condition2:
    # Code à exécuter si la condition2 est vraie
else:
    # Code à exécuter si aucune des conditions précédentes n'est vraie
```

Également pour les boucles **for** et **while**.
```python
for element in sequence:
    # Code à exécuter pour chaque élément de la séquence

while condition:
    # Code à exécuter tant que la condition est vraie
```

### Les fonctions utilisées

La première fonction que j'ai vu en python était **print** qui permet d'afficher n'importe quel object Python.

```python
print("Hello world")
>>> Hello world
print(5)
>>> 5
```
La deuxième fonction (importante) que j'ai pu découvrir était **input** qui permettait à l'utilisateur d'entrer des caractères aux clavier.
```python
input("Please input an integer: ")
```

**Autres:**
- **int(maVariable)** pour convertir une variable en integer
- **type(maVariable)** pour avoir le type de *maVariable*