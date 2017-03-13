# My Interactive ToDo List

Créer une todo list interactive à deux : 
* deux fronts
* un seul "backend" firebase


---

# Objectifs : 

* en tant qu'utilisateur, je peux ajouter un élément à la liste
* en tant qu'utilisateur A, je reçois "en temps réel", un élement ajouté à la liste par l'utilisateur B.
* en tant qu'utilisateur, je peux uploader des images
* en tant qu'utilisateur, je peux visualiser les images uploadées par les deux utilisateurs
* en tant qu'utilisateur, je peux supprimer un élément de la liste

---

Modèle et specs

## Item

```
item : {
	id
    	createdAt
    	content
    	status
}

```

Enregistré dans le noeud /items sous firebase Database

---

Modèle et specs

## Image

Enregistré dans le noeud /img sous firebase Storage

---

# Contraintes : 
* pas de CSS

---

# Bonus : 
* une page de création de compte
* une page de connexion
* ajouter des règles de sécurité
  * ne peut supprimer que les éléments à soi
  * sauf si l'élément a été créé il y a plus de 10 minutes
* mise à jour des éléments (fait ou à faire)