## 1. Contexte de l’application

L’ASBL **“Les Coccinelles”** est située à Morhet, un village dans la province du Luxembourg. Celle-ci met à disposition des habitants et personnes extérieures une salle à louer, et y organise régulièrement des événements afin de faire vivre le village. Des activités sont également organisées hors de la salle.

À l’heure actuelle, l’ASBL ne possède pas de logiciel pour être gérée. Afin de leur faire gagner du temps et de réduire la charge de travail des différents membres, je souhaite développer une application de gestion pour l’ASBL afin qu’il puisse y gérer :

- Les activités de l’ASBL
- Les articles concernant l’ASBL ou les activités
- La gestion de la salle du village
- La gestion des différents membres
- Les réservations de la salle
- Les messages de contact
- L’organisation des réunions

De plus, un site public sera développé afin de promouvoir leur image et mettre directement à disposition de l’utilisateur des informations concernant l’ASBL.

L’objectif est de fournir à l’ASBL un produit moderne et simple d’utilisation pour gérer au mieux tous les points énoncés ci-dessus.

## 2. Personas et parcours utilisateurs

### Adrien – Président de l’ASBL

**→ Rôle** : Président de l’ASBL

### 🗂️ Parcours utilisateur 1 – Réservation de la salle

Samedi matin, Adrien reçoit une notification comme quoi **Claude** voudrait réserver la salle de l’ASBL via un message envoyé depuis le site de l’ASBL. Il se rend alors sur son interface d’administration, se rend dans le section lié au message et commence à lire le message. Après avoir lu le message, il vérifie si les dates sont disponibles et se rend sur la page de création d’une réservation.

Un fois cette sur cette page, il clique sur le bouton “Créer une nouvelle réservation”, il indique ensuite les dates de début et fin de la réservation ainsi que les informations sur **Claude**. Il se rend ensuite dans la partie liée au détail technique de la salle, il choisit la salle à réserver ainsi que  le type de réservation parmi les types proposés et valide la réservation. Lors de la création de la fiche, un contrat à été généré en fonction du type de la réservation, il peut le télécharger après la création.

Une fois la fiche créée, un email est envoyé à **Claude** pour confirmer sa réservation.

---

### 🗂️ Parcours utilisateur 2 – Erreur dans la fiche

Deux jours plus tard, Adrien veut télécharger le contrat de location pour pouvoir le faire signer à **Claude.** Malheureusement, il se rend compte qu’il s’est trompé dans le type d’activité et en plus, il n’existe pas dans les types disponibles. Il clique alors sur le lien qui lui permet d’ajouter des types à la volée, il renseigne alors un nouveau type “Activités sportives” et lui attribue les informations nécessaires (Prix sans carte de membre, prix avec carte de membre), puis valide le nouveau type. Il peut ensuit régénérer le contrat avec les nouvelles informations.

Le nouveau type ajouté est visible et modifiable dans la page liée à la salle de l’ASBL.

---

### 🗂️ Parcours utilisateur 3 – Gestion de la salle

Adrien vient d’apprendre que la commune souhaite leur allouer une deuxième salle, il accepte donc avec grand plaisir.

Il se rend donc dans la page où toutes les salles sont listées, clique sur le bouton de création d’une salle et commence à remplir les informations ( *adresse* | *nom* | *logo* ). Elle y ajoute aussi des types de réservation comme sur la première salle.

Ensuite, elle doit renseigner les différentes interventions prévues dans la salle, elle y note donc qu’elle doit faire vérifier l’extincteur de la cuisine. Un rappel lui sera envoyé tous les x temps et sera aussi présent sur le tableau de bord.

---

### 🗂️ Parcours utilisateur 4 – Création d’un profil membre normal

Après avoir été satisfait par sa réservation, **Claude** décide de rejoindre l’ASBL pour y donner de son temps, il demande à Adrien qui accepte avec grand plaisir. Une fois rentré du travail, Adrien se rend sur l’interface d’administration, va dans la rubrique lié aux membres, et commence à créer un nouveau profil membre. Il remplit les informations et choisi son rôle dans l’ASBL. Une fois la création terminée, **Claude** reçoit un mail avec ses identifiants, accède à son compte et peut voir certaines informations sur le site.

---

### 🗂️ Parcours utilisateur 5 – Départ de Camille

Après 26 années passées dans l’ASBL, Camille décide de tirer sa révérence de de quitter cette belle aventure. Elle prévient Adrien qui va changer le statut de Camille en “Partie” dans l’application. Elle y garde toujours le profil de Camille au cas où elle décide de revenir un jour.

---

### Léa – Membre du comité

**→ Rôle** : Secrétaire de l’ASBL

### 🗂️ Parcours utilisateur 1 – Création d’une réunion

En tant que membre du comité de l’ASBL, Léa a le droit de planifier des réunions avec les membres de l’ASBL ( Tout rôle confondu ). Et justement, elle aimerait planifié une réunion pour parler de leur prochains événements.

Elle se rend donc sur la page de création d’une réunion, y inscrit le sujet, la date, l’endroit et sélectionne les participants parmi les membres de l’ASBL, elle valide la création de la réunion.

Une fois la réunion créée, elle décide d’y ajouter des documents pour préparer la future réunion en avance, une section dédiée a cette fonctionnalité est prévue dans l’application.

---

### 🗂️ Parcours utilisateur 2 – En pleine réunion

Lors de la réunion programmée par Léa, beaucoup de propositions ont été faites pour le futur événement. Une fois rentrée chez elle, elle remet tout au propre dans un nouveau document, et le rend disponible sur l’application. Tous les membres, peu importe le rôle, y ont accès mais seul le comité peut modifier les informations de la réunion.

Léa semble satisfaite du compte rendu de la réunion et décide de créer l’événement.

---

### 🗂️ Parcours utilisateur 3 – Un nouvel événement

Après cette longue réunion, Léa créer l’événement via une page dédié à cette action. Il y ajoute toutes les informations nécéssaires à la création de l’événement. Cette action engendre la publication de l’événement sur le site public de l’ASBL.

Un fois l’événement publié, Léa ajoute dans la liste des tâches à réaliser, les différentes choses à ne pas oublier lors de la préparation en amont de l’événement.

Après quelques semaines, de nombreux papiers se sont accumulés dans le bureau de Léa, elle décide donc de numériser tous les papiers et de les introduire dans le site dans la section dédiée à cet effet. Elle peut même y créer des dossiers pour mieux structurer tous ses papiers.

---

### Alex – Membre du comité

**→ Rôle** : Gestionnaire du site public

### 🗂️ Parcours utilisateur 1 – Changement d’adresse

L’annonce vient de tomber, la commune à décidé de changer le nom de la rue où se trouve l’asbl. Alex se rend alors dans les paramètres du site public dans l’administration et modifie l’adresse. Une fois la modification effectuée, elle est directement répercutée dans le site public. Il en profite par la même occasion pour mettre à jour le numéro de téléphone.

---

### 🗂️ Parcours utilisateur 2 – Compte rendu de la randonnée VTT annuelle

Tous les ans, l’asbl organise une randonnée VTT, cette année fut un succès ! Alex décide alors d’écrire un petit article sur cette édition afin de la partager à un grand nombre de personnes. Il se rend alors dans la page spécifique à la création d’articles dans son application et se met à rédiger. Il y ajoute plusieurs paragraphes, photos, etc.

---

### Flora – Simple utilisateur d’internet

**→ Rôle** : Simple visiteur

### 🗂️ Parcours utilisateur 1 – Réservation d’une salle

Flora cherche une salle pour l’anniversaire de son petit garçon. Son mari lui avait partagé le lien de cette salle. Elle y regarde donc, lit les informations et fait une demande de réservation. L’administrateur reçoit la demande dans son administration et donne des nouvelles à Flora par la suite.

---

### 🗂️ Parcours utilisateur 2 – Recherche d’une activité

Ce week-end, Flora a envie de bouger, elle regarde les activités que propose l’asbl. Elle tombe sur la randonnée VTT annuelle, elle décide donc d’y aller. Elle regarde les différentes distances proposées car elle compte y aller avec son fils mais celui-ci n’est pas très sportif et donc pas capable de réaliser une longue distance. Après avoir trouvé la distance qu’il lui convient, elle la partage a son mari pour voir si cela lui convient.

Après avoir fait la randonnée, Flora est vraiment très contente de l’organisation et décide donc de mettre une note (Étoile) sur l’activité proposée par l’asbl. Il est aussi possible d’y ajouter de vraies notes écrites mais toujours par validation de l’administration avant publication sur le site public.

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

- Informations sur les prochaines réunions, événements, réservations

---

### 🧩 Gestion des activités – événements

- Création, suppression, modification de l’événement
- Liste des choses importantes à réaliser
- Classement de fichiers selon des dossiers
- Note des utilisateurs publics (Toujours une validation via l’admin)

---

### 🤵‍♂️ Gestion des membres

- Création, suppression, modification de profil membre
- Différents rôles (Comité ou simple membre)

---

### 📆 Gestion des réunions

- Création, suppression, modification d’une réunion
- Ajout de fichiers, photos (Triage avec dossier)
- Sélection des participants

---

### 🌐 Site public

- Page d’accueil
- Page de présentation de l’asbl
- Page d’informations sur la salle + formulaire de demande de réservation
- Page de contact (Demande d’informations ou devenir bénévole)
- Page des événements à venir
- Page d’actualités (Retour sur les événements)

---

## 4. Technologies

- **Back-End** : Laravel 12 + Livewire 4
- **Front-End** : Laravel 12 + Tailwind CSS + Alpine.js – JavaScript natif
- **Base de données** : MySQL
- **Testing** : Pest
- **Stockage** : AWS S3 Storage
- **Hébergement** : Laravel Cloud + Infomaniak