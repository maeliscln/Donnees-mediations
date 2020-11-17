# Étude du phénomène “*d’airbnbsation*” à Aix-en-Provence

Plus de douze ans après sa création, la plateforme communautaire [*Airbnb*](https://www.airbnb.fr/) a révolutionné le marché de l’hébergement touristique en mettant en relation des particuliers proposant et recherchant un logement à la location. Si un tel succès s’explique avant tout par les avantages économiques induits par ce système, il n’est pas sans conséquence tant sur le **marché du tourisme** que sur celui de **l’immobilier**. *Airbnb* s’est ainsi souvent trouvée sous le feu des critiques : accusée de causer une pénurie de logements pour les résidents permanents, notamment dans les villes à forte attraction touristique où de plus en plus de logements sont entièrement dédiés à la location touristique de courte durée sur *Airbnb*, la plateforme serait également à l’origine d’une hausse du prix de l’immobilier dans ces grandes villes. C’est ce phénomène, parfois désigné sous le terme “*d’airbnbisation*”, auquel nous nous sommes intéressés pour réaliser cette note d’étude. 

**Il s’agira donc d’explorer le lien entre la hausse du prix de l’immobilier à Aix-en-Provence sur les quatre dernières années et la hausse du nombre de logements *Airbnb* dans la même ville et sur la même période.**


## Une double augmentation du prix de l’immobilier et du nombre de logements *Airbnb* à Aix-en-Provence

À partir des jeux de données que nous avons récoltés respectivement sur [**data.gouv**](https://www.data.gouv.fr) et sur [**l’Observatoire Airbnb**](http://observatoire-airbnb.fr) puis exploités, nous avons fixé deux indicateurs : le prix moyen des biens immobiliers à l’achat à Aix-en-Provence (à partir des données DVF) et le nombre de logements *Airbnb* disponibles à la location à Aix-en-Provence entre 2016 et 2019. Nous avons ainsi créé deux graphiques linéaires distincts afin de montrer l’évolution de ces données au fil des années. 

Sur le **premier graphique**, nous pouvons constater que **le nombre de logements *Airbnb* augmente de manière graduelle entre 2016 et 2019** avec **un taux d’augmentation annuel moyen de 33,28%**.

![Évolution du nombre de logements Airbnb à Aix-en-Provence](https://raw.githubusercontent.com/maeliscln/Donnees-mediations/main/E%CC%81volution%20du%20nombre%20de%20logements%20Airbnb%20a%CC%80%20Aix-en-Provence.png)

Sur le **deuxième graphique**, nous pouvons constater, en parallèle, une augmentation du prix de la valeur foncière entre 2016 et 2019. Si entre 2016 et 2017, le taux d’augmentation est de 14,24%, ce dernier perd en valeur par la suite pour connaître un taux d’augmentation annuel moyen de 9%. Suite à ces premières analyses de données, nous remarquons donc une augmentation à la fois pour le nombre de logements *Airbnb* et le prix de l'immobilier à Aix-en-Provence. À ce stade, il s’agit de déterminer si une causalité peut être établie entre ces deux augmentations.

![Évolution du prix moyen des biens immobiliers à l'achat à Aix-en-Provence](https://raw.githubusercontent.com/maeliscln/Donnees-mediations/main/E%CC%81volution%20du%20prix%20moyen%20des%20biens%20immobiliers%20a%CC%80%20l'achat%20a%CC%80%20Aix-en-Provence%20(en%20%E2%82%AC%2C%20divise%CC%81%20par%20100).png)

## La ville d'Aix-en-Provence est-elle sujette à "*l'airbnbsation*" ?

Si la lecture des deux premiers graphiques linéaires nous a donc permis de mettre en évidence une évolution croissante à la fois du nombre de logements *Airbnb* et du prix de l’immobilier, qui nous a conduit à formuler l’hypothèse de l’existence d’un phénomène d’*airbnbisation* à Aix-en-Provence, ce troisième graphique nous invite à **rester prudent** quant à une potentielle corrélation entre ces deux variables. Le diagramme en bâtons ici généré permet en effet une meilleure visualisation de l’écart d’augmentation entre les deux variables : on constate que celle-ci est loin d’être proportionnelle, **le nombre de logements *Airbnb* ayant augmenté de façon bien plus importante sur les quatre dernières années que le prix de l’immobilier aixois**. L’influence de l’un sur l’autre reste donc entièrement à prouver.

![Nombre de logements Airbnb en location et prix moyen des biens immobiliers à l'achat à Aix-en-Provence](https://raw.githubusercontent.com/maeliscln/Donnees-mediations/main/Nombre%20de%20logements%20Airbnb%20en%20location%20et%20prix%20moyen%20des%20biens%20immobiliers%20a%CC%80%20l'achat%20a%CC%80%20Aix-en-Provence.png)

En calculant le pourcentage d’augmentation pour nos deux indicateurs entre 2016 et 2019, cette absence de proportionnalité est d’autant plus flagrante : le prix de l’immobilier à Aix-en-Provence a en effet augmenté de 29% entre 2016 et 2019, augmentation certes considérable mais qui apparaît moindre quand on la compare à l’augmentation de 136% du nombre de logements *Airbnb* à Aix-en-Provence entre 2016 et 2019.

## L'influence des zones géographiques

Nous voulions produire des visualisations de données qui contenaient une composante géographique, afin de montrer, le cas échéant, si certains quartiers d’Aix-en-Provence subissent davantage que d’autres les effets de l’*airbnbsation*. Nous avons d’abord réalisé une simple carte grâce au logiciel [**Khartis**](https://www.sciencespo.fr/cartographie/khartis) développé par Sciences Po Paris pour comprendre où se situaient tous les logements *Airbnb* disponibles en octobre 2016, grâce aux coordonnées géographiques contenues dans notre jeu de données initial (latitude et longitude). 

**Voici le résultat obtenu :**

![Localisation des logements Airbnb disponibles à Aix-en-Provence](https://raw.githubusercontent.com/maeliscln/Donnees-mediations/main/Localisation%20des%20logements%20Airbnb%20disponibles%20a%CC%80%20Aix-en-Provence%20(2016).png)

Le problème de cette visualisation est qu’elle ne nous donne **aucune information sur la répartition géographique des logements** en fonction des sections cadastrales. Cela ne nous permet donc pas de savoir quels peuvent être les logements situés dans le centre-ville d’Aix-en-Provence qui auraient éventuellement pu être disponibles pour des locations étudiantes s’ils n’avaient pas été destinés à la location *Airbnb*.

Pour cela, nous avons donc récupéré un jeu de données qui listait les sections cadastrales à l’échelle de la municipalité d’Aix-en-Provence, ce qui nous a permis de calculer, grâce à un tableau croisé dynamique, combien de logements *Airbnb* comprenait chaque section cadastrale.

Enfin, nous avons récupéré un jeu de données au format **.geojson** qui nous permettait d’importer, dans **Khartis**, un fond de carte par sections cadastrales. Ainsi, nous avons pu exploiter notre jeu de données pour faire varier les couleurs sur notre carte finale en fonction d’un critère essentiel : le nombre de logements *Airbnb* disponibles par section cadastrale. 

**En voici le résultat :**

![Nombre de Airbnb par section cadastrale à Aix-en-Provence](https://raw.githubusercontent.com/maeliscln/Donnees-mediations/main/Nombre%20de%20logements%20Airbnb%20par%20section%20cadastrale%20(2017).png)

Grâce à cette dernière visualisation, nous constatons donc que les parcelles qui concentrent le plus de logements Airbnb sont **les 13 sections cadastrales qui composent le centre-ville**. Nous pensions, à l’origine, que beaucoup de logements disponibles à la location sur Airbnb seraient plutôt des logements aux surfaces généreuses, comme des villas familiales situées aux alentours d’Aix-en-Provence. En fait, ce qui ressort de la dernière carte confirme plutôt l’idée selon laquelle *Airbnb* vient **aggraver la pénurie de logements étudiants dans le centre-ville d’Aix**, car la majorité du parc de logements disponible sur Airbnb concerne des studios dans le centre-ville. Il est certainement plus rentable pour les propriétaires de consacrer leurs logements à la location touristique sur Airbnb plutôt qu’à des locations étudiantes annuelles. Pour autant, ces studios manquent pour de nombreux étudiants qui se voient obligés d’habiter en périphérie d’Aix-en-Provence, faute d’avoir réussi à trouver un logement dans le centre-ville. Notons cependant que la crise sanitaire, qui a fortement attaqué le secteur touristique, permettra peut-être d’inverser la tendance.

## La boîte noire

Une boîte noire, pour conclure, afin de mettre en exergue les difficultés rencontrées pendant cette étude.

- **Première difficulté** : un problème s'est posé lorsque nous avons voulu exploiter les données sur la valeur foncière de **data.gouv** car nous avons remarqué un fort écart de prix entre 2018 et 2019. Il s’agissait d’une augmentation bien trop importante pour être vérifiée dans les faits, ce qui nous a poussés à questionner la fiabilité de la base de données. En parcourant le tableau, nous nous sommes rendus compte que de nombreux doublons apparaissent. En fait, ces doublons étaient le résultat d’une duplication des dispositions par mutations : par exemple, la mutation (le bien immobilier) numéro 2013P00181 correspondait à 8 dispositions, soient autant de parcelles qui composent le bien. Dès lors, il s’agissait de dédupliquer puis de recalculer les moyennes de prix pour chaque année. Pour cela, nous avons utilisé l’outil [**workbenchdata.com**](https://workbenchdata.com).

- **Deuxième difficulté** : un autre problème, d'échelle cette fois, se posait pour le troisième graphique. Les valeurs oscillant entre 2.000 et 6.000 pour le nombre de *Airbnb* contre 200.000 à 400.000 pour les valeurs DVF, il apparaissait difficile de les regrouper de façon lisible dans un seul et même graphique. Nous avons donc fait le choix de renseigner les valeurs DVF **en € divisé par 100** afin qu’elles rentrent dans la même échelle que le nombre de logements *Airbnb*.
