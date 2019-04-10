# API 
Cette api permet de récupérer les entreprises ayant effectué un acte d'augmentation de capital social.

Elle dispose pour le moment d'une seule route vous permettant d'obtenir ces entreprises.

Routes: 

# GET http://ip:port/getEntreprises/nbJoursMaxdeLacte
+ Response 200 (text/plain)

Exemple d'appel pour recevoir la liste des entreprises ayant déposé leur acte d'augmentation de capital il y a moins de 30 jours:

```http://ip:port/getEntreprises/30```

Réponse: 
Une string contenant un tableau d'objets sous cette forme:
```
[
    {
    dateActe: '2018-12-20T00:00:00.000Z',
    adresse: '28 BOULEVARD GEORGES CLEMENCEAU  21000 DIJON',
    dateImmat: '30/06/1919',
    naf: '6820A : Location de logements',
    Effectif: ' Comptes annuels déposés au Greffe. Commande possible. ',
    'Résultat': '31/12/2016',
    CA: ' Comptes annuels déposés au Greffe. Commande possible. ',
    'Clôture': '31/12/2017',
    greffe: 'DIJON',
    statut: 'R.C.S.',
    url: 'https://www.infogreffe.fr/entreprise-societe/15450638-societe-anonyme-d-habitations-a-loyer-modere-habellis-210454B000630000.html?typeProduitOnglet=EXTRAIT&afficherretour=false',
    name: 'SOCIETE ANONYME D\'HABITATIONS A LOYER MODERE HABELLIS' 
    },
    dateActe: '2018-12-20T00:00:00.000Z',
    adresse: '28 BOULEVARD GEORGES CLEMENCEAU  21000 DIJON',
    dateImmat: '30/06/1919',
    naf: '6820A : Location de logements',
    Effectif: ' Comptes annuels déposés au Greffe. Commande possible. ',
    'Résultat': '31/12/2016',
    CA: ' Comptes annuels déposés au Greffe. Commande possible. ',
    'Clôture': '31/12/2017',
    greffe: 'DIJON',
    statut: 'R.C.S.',
    url: 'https://www.infogreffe.fr/entreprise-societe/15450638-societe-anonyme-d-habitations-a-loyer-modere-habellis-210454B000630000.html?typeProduitOnglet=EXTRAIT&afficherretour=false',
    name: 'SOCIETE ANONYME D\'HABITATIONS A LOYER MODERE HABELLIS' 
]


