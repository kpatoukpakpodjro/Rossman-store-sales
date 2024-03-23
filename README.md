# Rossman-store-sales
Prédiction

Rossmann exploite plus de 3 000 pharmacies dans 7 pays européens. Actuellement, les gérants des magasins Rossmann sont chargés de prévoir 
leurs ventes quotidiennes jusqu'à six semaines à l'avance. Les ventes en magasin sont influencées par de nombreux facteurs, 
notamment les promotions, la concurrence, les vacances scolaires et nationales, la saisonnalité et la localité.
Avec des milliers de managers individuels prédisant les ventes en fonction de leur situation unique, la précision des résultats peut être très variable.
Champs de données
La plupart des champs sont explicites. 
* Id - un identifiant qui représente un double (Store, Date) dans l'ensemble de test
* store - un identifiant unique pour chaque magasin
* sales - le chiffre d'affaires pour un jour donné (c'est ce que vous prédisez)
* Customers  - le nombre de clients un jour donné
* Open - un indicateur indiquant si le magasin était ouvert : 0 = fermé, 1 = ouvert
* StateHoliday - indique un jour férié. Normalement, tous les magasins, à quelques exceptions près, sont fermés les jours fériés.
   A noter que toutes les écoles sont fermées les jours * fériés et les week-ends. a = jour férié, b = vacances de Pâques, c = Noël, 0 = aucun
* SchoolHoliday - indique si le (Magasin, Date) a été affecté par la fermeture des écoles publiques
* StoreType  - différencie 4 modèles de magasins différents : a, b, c, d
* Assortiment - décrit un niveau d'assortiment : a = basique, b = extra, c = étendu
* CompetitionDistance - distance en mètres jusqu'au magasin concurrent le plus proche
* CompetitionOpenSince[Mois/Année] - donne l'année et le mois approximatifs de l'ouverture du concurrent le plus proche.
* Promo : indique si un magasin propose une promotion ce jour-là.
* Promo2 - Promo2 est une promotion continue et consécutive pour certains magasins : 0 = le magasin ne participe pas, 1 = le magasin participe
* Promo2Since[Year/Week] : décrit l'année et la semaine civile au cours desquelles le magasin a commencé à participer à Promo2.
* PromoInterval - décrit les intervalles consécutifs de démarrage de Promo2, en nommant les mois pendant lesquels la promotion est relancée.
  Par exemple, « février, mai, août, novembre » signifie que chaque cycle commence en février, mai, août et novembre d'une année donnée pour ce magasin.
