# Emplacements de Paiements

----------

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td><strong>Who can use this feature?</strong></td><td><span data-gb-custom-inline data-tag="emoji" data-code="2714">✔</span><mark style="color:red;">Revendeurs de Paiements</mark></td><td></td></tr></tbody></table>

La section 'Emplacement de paiements' dans le Portail des Revendeurs est cruciale pour les Revendeurs. Elle leur permet de créer un 'Emplacement de paiements' puis d'inviter l'Utilisateur à y accéder. Cet emplacement créé sert d'espace de travail dédié, donnant accès aux fonctionnalités du Portail de Paiements.

## Créer des Emplacements de Paiements

Voici le processus petit à petit pour activer l'accès des Utilisateurs de paiements à unTill Payments :

1. L'Utilisateur des paiements lance une demande dans le Back Office.
2. Le Revendeur des paiements est notifié de cette demande par email.
3. Le Revendeur des paiements crée un 'Emplacement de paiements'.
4. Après cela, le Revendeur des paiements envoie une invitation à l'Utilisateur des paiements.
5. En acceptant l'invitation, l'Utilisateur des paiements peut accéder au Portail de Paiements.

Les Revendeurs ont la opportunité d'ajouter ou de supprimer des Emplacements de Paiements de leur liste et d'inviter des Utilisateurs en conséquence.

Il est à noter que pour chaque Emplacement de Paiements, vous avez la possibilité d'inviter plusieurs Utilisateurs directement.

## Deux types de frais

Dans la section 'Emplacement de paiements', les Revendeurs peuvent configurer à la fois les 'Frais de traitement' et les 'Frais d'acquisition'. Ces frais seront appliqués après qu'une transaction soit acceptée. Lorsqu'un client effectue un paiement en utilisant n'importe quelle méthode, la transaction est traitée, et la division des frais entre les partieies impliquées commence.

En fonction des accords entre le Revendeur et l'Utilisateur des paiements, ces deux types de frais ('Frais de traitement' et 'Frais d'acquisition') sont définis par le Revendeur. Après la signature du contrat, ils commencent à fonctionner et à recevoir des paiements.

Les 'Frais de traitement' et les 'Frais d'acquisition' sont déduits du montant qui a été accepté. La Plateforme Adyen détient ces frais jusqu'au moment où la division se produit.

| Type de frais    | Caractéristiques de la valeur                                                |
| ---------------- | ---------------------------------------------------------------------------- |
| Frais de traitement | Il est défini en centimes, avec une valeur minimale de €0,07 et une valeur maximale de €0,11 |
| Frais d'acquisition | Il est défini en pourcentage, avec une valeur minimale de 0,5 % et une valeur maximale de 1 % |

{% hint style="info" %}
Pour plus d'informations sur les paiements, référez-vous à cette page.
{% endhint %}

### Frais de traitement

La division des 'Frais de traitement' implique deux parties :

* unTill
* Revendeur

#### Partie d'unTill

unTill facture des frais fixes pour chaque transaction. Pour les 'Frais de traitement', ces frais fixes sont de €0,07 par transaction.

#### Partie du Revendeur

La partie du Revendeur des 'Frais de traitement' peut varier en fonction des accords pris avec l'Utilisateur des paiements qui accepte des conditions spécifiques pour la configuration de l'Emplacement de paiements.

Prenons un exemple : Si un Utilisateur des paiements accepte des 'Frais de traitement' de €0,1, le Revendeur recevra €0,03 après la déduction d'unTill (€0,1 - €0,07).

Une fois la division des frais terminée, la Plateforme Adyen crédite ce montant au 'Solde courant' du Revendeur.

### Frais d'acquisition

Le 'Frais d'acquisition' suit une structure similaire aux 'Frais de traitement' pour la division et le transfert des revenus. Cependant, dans cette phase, l'Utilisateur des paiements reçoit une partieie des fonds, qui sont crédités à leur 'Solde courant'.

La division du 'Frais d'acquisition' implique trois parties :

* unTill
* Revendeur
* Utilisateur des paiements

#### Partie d'unTill

Comme pour les 'Frais de traitement', unTill facture des frais fixes pour chaque transaction. Pour les 'Frais d'acquisition', unTill déduit 0,45 % du montant total.

#### Partie du Revendeur

La partie du Revendeur est basée sur la valeur définie dans la section 'Emplacement de paiements', selon leur accord avec l'Utilisateur des paiements. Le frais crédité au 'Solde courant' du Revendeur sera réduit par la partie d'unTill.

Prenons un exemple : Si le Revendeur fixe un 'Frais d'acquisition' de 0,6 %, après déduction de la partie d'unTill, le Revendeur recevra 0,15 % du montant total (0,6 % - 0,45 %).

#### Partie de l'Utilisateur des paiements

Le calcul de la partie de l'Utilisateur des paiements est simple. Du montant total de la transaction, soustrayez les parties d'unTill et du Revendeur. La plateforme Adyen déduit également un 'Frais de paiement' du 'Solde courant' de l'Utilisateur des paiements.

### Exemple

Prenons un exemple : Supposons qu'un client dans un restaurant paye €10. En prenant l'exemple du 'Frais de traitement', le frais total (€0,1) est répartiei entre les 'Soldes courants' d'unTill et du Revendeur. Le 'Frais d'acquisition', dans l'exemple donné (0,6 % du montant total), s'élève à €0,06. Après déduction de ces frais, la partie de l'Utilisateur des paiements devient €9,84.

{% hint style="warning" %}
**Remarque :** Après cette division, Adyen réduira davantage la partie de l'Utilisateur des paiements en retirant le frais de transaction de son 'Solde courant'.
{% endhint %}

### Déduction de la TVA pour les Utilisateurs des paiements des Pays-Bas

Les Utilisateurs des paiements des Pays-Bas sont soumis à une charge de TVA supplémentaire. Ces fonds de TVA sont d'abord dirigés vers unTill, qui est responsable de la gestion des paiements de TVA pour les activités commerciales en cours dans le pays.

Par la suite, unTill attribue une partieie de ces fonds de TVA au Revendeur, en fonction des paiements de TVA effectués par l'Utilisateur des paiements.


