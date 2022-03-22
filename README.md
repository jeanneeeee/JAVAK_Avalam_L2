1) Placez vous dans le répertoire lié à l'archive ;
2) Exécutez 'make' ;
3) Placez vous dans le répertoire tournoi ;

-- POUR JOUER UN TOURNOI --
4) Ouvrez deux terminaux. Dans chacun d'eux, exécutez 'source dyn.sh'. 
Cela exécute les commandes du fichier dyn.sh dans le shell courant, ce qui permet d'ajouter une variable d'environnement (LD_LIBRARY_PATH) pour indiquer le chemin des librairies externes.
5) Dans le premier terminal, exécutez ./bin/moteur.exe 1 (1 s/coup) ;
6) Dans le second terminal, exécutez ./genJoueurs.sh 5, ce qui inscrit 5 joueurs nommés joueur<N>.exe au tournoi ;
7) Ouvrez le répertoire tournoi/web avec votre explorateur de fichiers... et double-cliquez sur avalam-tournoi.html.
8) Appuyez sur ENTREE dans le terminal exécutant moteur.exe ;


-- POUR JOUER UN DUEL --
4) Ouvrez trois terminaux. Dans chacun d'eux, exécutez 'source dyn.sh' ;
5) Dans le premier terminal, exécutez ./bin/duel.exe ; 
6) Dans le second terminal, exécutez un premier joueur ; 
7) Dans le second terminal, exécutez un second joueur.

Si vous désirez jouer contre un moteur de jeu, vous pouvez choisir les joueurs 'humain1.exe' (saisie des indices des coups) ou 'humain2.exe' (saisie des cases de départ et d'arrivée du coup). Il faudra jouer dans le temps imparti, sauf si le temps du joueur est affecté à la durée 0. Dans ce cas, il faudra jouer avec humain3. C'est ce qui est utilisé pour la partie finale humain-machine lors de la soutenance. 

8) Appuyez sur ENTREE dans le terminal exécutant duel.exe ;
9) Indiquez les temps de réflexion de chaque joueur au clavier ;
10) Appuyez à nouveau sur ENTREE pour démarrer la première partie du duel ;
11) Ouvrez le répertoire tournoi/web avec votre explorateur de fichiers... et double-cliquez sur avalam-tournoi.html ;
12) Après chaque partie du duel, vous pourrez indiquer si vous voulez poursuivre le duel ou non.

-- POUR JOUER UN DUEL "INSTANTANE" --
Répétez les opérations précédentes, en choisissant ./bin/duel-instantane.exe ; et des joueurs "instantanes". Ces joueurs jouent comme les autres mais doivent appeler la fonction finaliserCoup() lorsqu'ils ont terminé.  

---------------------------------

Si jamais vous tuez le process moteur ou duel, il se peut que des process joueurs continuent de s'exécuter. 
Il faut alors invoquer ./killjoueurs.sh avant de recommencer un tournoi

