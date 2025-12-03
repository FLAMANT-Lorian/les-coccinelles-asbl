# Projet de fin d’études

# Cahier des charges – Application de gestion d’une ASBL

## 1. Contexte de l’application

- Un site ADMIN
- Un site Public

## 2. Personas et parcours utilisateurs

### Adrien – Président de l’ASBL

**→ Rôle** : Président de l’ASBL

### 🗂️ Parcours utilisateur 1 – Réservation de la salle

Samedi matin, Adrien reçoit une notification comme quoi **Claude** voudrait réserver la salle de l’ASBL via un message envoyé depuis le site de l’ASBL. Il se rend alors sur son interface d’administration, se rend dans le section lié au message et commence à lire le message. Après avoir lu le message, il vérifie si les dates sont disponibles et se rend sur la page de création d’une reservation.

Un fois cette sur cette page, il clique sur le bouton “Créer une nouvelle réservation”, il indique ensuite les dates de début et fin de la réservation ainsi que les informations sur **Claude**. Il se rend ensuite dans la partie lié au détail technique de la salle, il choisi la salle à reserver ainsi que  le type de réservation parmi les types proposées et valide la réservation. Lors de la création de la fiche, un contrat à été générer en fonction du type de la réservation, il peut le télécharger après la création.

Une fois la fiche créer, un email est envoyé à **Claude** pour confirmer sa réservation.

---

### 🗂️ Parcours utilisateur 2 – Erreur dans la fiche

Deux jours plus tard, Adrien veut télécharger le contrat de location pour pouvoir le faire signer à **Claude.** Malheureusement, il se rend compte qu’il s’est trompé dans le type d’activité et en plus, il n’existe pas dans les types disponibles, il clique alors sur le lien qui lui permet d’ajouter des types à la volés, il renseigne alors un nouveau type “Activités sportives” et lui attribut les informations nécéssaire (Prix sans carte de membre, prix avec carte de membre), puis valide le nouveau type. Il peut ensuit régénérer le contrat avec les nouvelles informations.

Le nouveau type ajouté est visible et modifiable dans la page lié à la salle de l’ASBL.

---

### 🗂️ Parcours utilisateur 3 – Gestion de la salle

Adrien vient d’apprendre que la commune souhaite leur allouer une deuxième salle, il accepte donc avec grand plaisir.

Il se rend donc dans la page où toutes les salles sont listées, clique sur le bouton de création d’une salle et commence à remplir les informations ( *adresse* | *nom* | *logo* ). Elle y ajoute aussi des types de réservation comme sur la première salle.

Ensuite, elle doit renseigner les différentes intervention prévu dans la salle, elle y note donc qu’elle doit faire vérifier l’extincteur de la cuisine. Un rappel lui sera envoyé tout les x temps et sera aussi présent sur le tableau de bord.

---

### 🗂️ Parcours utilisateur 4 – Création d’un profil membre normal

Après avoir été satisfait par sa réservation, **Claude** décide de rejoindre l’ASBL pour y donner de son temps, il demande à Adrien qui accepte avec grand plaisir. Une fois rentré du travail, Adrien se rend sur l’interface d’administration, va dans la rubrique lié aux membres, et commence à créer un nouveau profil membre. Il rempli les informations et choisi son rôle dans l’ASBL. Une fois la création terminée, **Claude** reçoit un mail avec ses identifiants, accède à son compte et peut voir certaines informations sur le site.

---

### 🗂️ Parcours utilisateur 5 – Départ de Camille

Après 26 années passées dans l’ASBL, Camille décide de tirer sa révérence de de quitter cette belle aventure. Elle préviens Adrien qui va changer le statut de Camille en “Partie” dans l’application. Elle y garde toujours le profil de Camille au cas elle décide de revenir un jour.

---

### Léa – Membre du comité

**→ Rôle** : Secrétaire de l’ASBL

### 🗂️ Parcours utilisateur 1 – Création d’une réunion

En tant que membre du comité de l’ASBL, Léa a le droit de planifier des réunions avec les membres de l’ASBL ( Tout rôle confondu ). Et justement, elle aimerait planifié au réunion pour parler de leur prochains événements.

Elle se rend donc sur la page de création d’une réunion, y inscrit le sujet, la date, l’endroit et sélectionne les participants parmi les membres de l’ASBL, elle valide la création de la réunion.

Une fois la réunion créée, elle décide d’y ajouter des documents pour préparer la future réunion en avance, une section dédié a cette fonctionnalité est prévu dans l’application.

---

### 🗂️ Parcours utilisateur 2 – En pleine réunion

Lors de la réunion programmé par Léa, beaucoup de proposition ont été faites pour le futur événement. Une fois rentré chez elle, elle remet tout au propre dans un nouveau document, et le rend disponible sur l’application, tout les membres peut importe le rôle y ont accès mais seul le comité peut modifier les informations de la réunion.

Léa semble satisfaite du compte rendu de la réunion et décide de créer l’événement.

---

### 🗂️ Parcours utilisateur 3 – Un nouvel événement

Après cette longue réunion, Léa créer l’événement via une page dédié à cette action. Il y ajoute toute les informations nécéssaire à la création de l’événement. Cette action engendre la publication de l’événement sur le site public de l’ASBL.

Un fois l’événement publié, Léa ajoute dans la liste des tâches à réaliser les différentes choses à ne pas oublier lors de la préparation en amont de l’événement.

Après quelques semaines, de nombreux papiers se sont accumulés dans le bureau de Léa, elle décide donc de numériser tout les papiers et de les introduire dans le site dans la section dédié à cet effet. Elle peut même y créer des dossiers pour mieux structurer tout ses papiers.

---

## 3. Fonctionnalités

### ✉️ Envoi de notifications – mail

- Lorsqu’un événement approche
- Lorsqu’une réservation approche
    - Au locataire
- Lorsqu’une réunion approche

### 🗓️ Réservation de la salle

- Création, suppression, modification de la salle
- Création d’un contrat en fonction du type

---

### 🗓️ Calendrier

- Informations sur les prochaines réunions, événements, réservation

---

### 🧩 Gestion des activités – événements

- Création, suppression, modification de l’événement
- Liste des choses importantes à réaliser
- Classement du fichiers selon des dossiers

---

### 🤵‍♂️ Gestion des membres

- Création, suppression, modification de profil membre
- Différents rôles (Comité ou simple membre)

---

### 📆 Gestion des réunions

- Création, suppression, modification d’une réunion
- Téléversesement de fichiers, photos (Triage avec dossier)
- Sélection des participants

---

### 🌐 Site public

## (Possibilité de faire avec Wordpress ?? Si oui faire un persona pour le gestionnaire du site internet)

- Page d’accueil
- Page de présentation
- page de contact / réservation
- Page des événements
