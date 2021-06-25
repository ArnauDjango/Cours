 ![python](https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg)

## Listes

### Acceder a liste
` list[len(list) - 1] ` va au derniere element de la liste
### Supprimer la liste
` list.clear() ` liste vide

### Modifier la liste
#### Ajouter
` list.insert(2, "valeur")` inserer une valeur sur l ellement 2 de la liste  
` list[2:4] = ["Pierre", "Paul"] ` insert une suite de valeur a l'interieur de la liste  
` list.append("more")` ajoute une nouvelle valeur au bout de la liste  
` list.extend(["Jojo", "Bernard"])` ajoute plusieur valeurs
#### Supprimer
` del list[1] ` suprrime le deuxieme element de la liste  
` list.pop(1) ` même chose  
`list.remove("Jojo")` la premiere valeur "Jojo" sera supprimer de la liste

#### Split
petit fonction bien utile
```
text = input("Salut entre une chaine de la forme (email-pseudo-mdp)").split("-")
print(text)
print("Salut {}, ton email est {}, et le mdp = {}".format(text[1], text[0], text[2]))
```

### Modules

#### statics
```
import statics 

notes = [
    8, 12, 10,
    9, 4, 20,
]

print(notes)
print(notes[0])

result = statistics.mean(notes)

print(result)

```
le result donnera la moyenne des notes

#### random

##### randint
```
import random

for i in range(0, 100):
    valeur = random.randint(0, 100)
    print(valeur)
```
##### shuffle
Cette fonction du module random sert a mélange une liste
` random.shuffle(notes) `

## boucles

### for
```
for num_client in range(1, 6):
    print("Vous etes le client nº ", num_client)

# blacklist

blacklist = ['arnaud@gmail.com']

# for each: pour chaque valeur d'une liste donnée
emails = [ 'arnaud@gmail.com', 'dimitri@gmail.com', 'rosane@gmail.com', 'nikita@gmail.com']

for email in emails:
    if email in blacklist:
        print("Email {} banni, envoi impossible".format(email))
        continue # passe au prochain for 
    print("Email envoyé a : " , email)

#break sort de la boucle
```



