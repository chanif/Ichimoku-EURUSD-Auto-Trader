# Ichimoku-EURUSD-Auto-Trader
Ichimoku EURUSD Auto Trader for Metatrader 5

Utilisation :
Attacher cet EA à un graphique EURUSD en unité de temps 15 minutes dans Metatrader 5.
(Par sécurité, même si vous attachez cet EA à un graphique qui n'est pas EURUSD, cet EA travaillera quand même sur EURUSD, et même si vous n'attachez pas cet EA à un graphique 15 minutes, et bien il travaillera quand même en 15 minutes).

Mises en garde :
Ne modifier la taille du lot qu'en fonction du capital investi. Je conseille de paramétrer la taille du lot à 1 pour un capital investi de 10000€ et à 0.1 pour un capital investi de 100€ par exemple.

Je déconseille de laisser un trade ouvert le vendredi soir avant la fermeture des marchés ; En effet, un gap à l'ouverture du lundi est toujours dangereux.

Je conseille de fermer une position dès qu'elle est en profit ; En effet, il n'est pas certain que le take profit soit atteint, même si le take profit paramétré par défaut a été optimisé suite à de nombreux tests exclusivement effectués sur l'EURUSD.

Caractéristiques :
Fonctionne sur compte réel et compte de démo, dans Metatrader 5.
Fonctionne en backtesting dans Metatrader 5.
Ne prend qu'un seul trade à la fois (tant qu'il y a un trade en cours, il n'y aura pas d'autre trade d'ouvert).
Fonctionne sur l'unité de temps 15 minutes et uniquement sur la paire EURUSD.
Trade 0.1 lot par défaut (Paramètre modifiable lorsqu'on attache l'EA à un graphique).
Envoi de notifications au(x) Metaquotes-ID qui sont saisis dans Metatrader 5 (s'il y en a de saisi).
Date d'expiration au 1er Juin 2017.

Critères Ichimoku :
Critères sur l'unité de temps 15 minutes :
Le tick en cours correspond à une nouvelle bougie.
Et La ligne SSA du Kumo en est au-dessus de la ligne SSB du kumo.
Et le plus haut de la bougie n-2 est au-dessus de la ligne SSA(-2) du kumo.
Et le plus bas de la bougie n-2 est sous la ligne SSA(-2) du kumo.
Et la bougie n-1 est au-dessus de la ligne SSA(-1) du kumo (le plus haut et plus bas sont au-dessus).
Critères sur l'unité de temps 5 minutes :
Et La Chikou Span n-26 est au-dessus de SSA(-26).
Et CS(-26) est au-dessus de SSB(-26).
Et CS(-26) est au-dessus de Tenkan Sen(-26).
Et CS(-26) est au-dessus de Kijun Sen(-26).
Et la bougie n-1 est au-dessus de SSA(-1) (le plus haut et plus bas sont au-dessus).
Et la bougie n-1 est au-dessus de SSB(-1) (le plus haut et plus bas sont au-dessus).
Et la bougie n-1 est au-dessus de TS(-1) (le plus haut et plus bas sont au-dessus).
Et la bougie n-1 est au-dessus de KS(-1) (le plus haut et plus bas sont au-dessus).

Performances :
Sur la période du 1er janvier 2016 au 26 janvier 2017, avec un paramétrage du lot à 1, et avec un dépôt initial de 10000€, le compte se retrouve à 13041€, soit une performance de +30% sur 1 an et 26 jours, avec un total de 91 trades, dont 25 trades perdants et 66 trades gagnants, soit 27% de trades perdants et 73% de trades gagnants.

Sur la période du 1er janvier 2017 au 26 janvier 2017, avec un paramétrage du lot à 1, et avec un dépôt initial de 10000€, le compte se retrouve à 10527€, soit une performance de +5.27% sur 26 jours, avec un total de 4 trades dont 1 perdant et 3 gagnants, soit 25% de trades perdants et 75% de trades gagnants.

