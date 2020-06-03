Ce qui a été fait pour tester le composant A2601

CREATION DU PROJET VIVADO :
	- ajouter tous les fichiers VHDL de chaque dossier (A2601, A6500(cpu),  A6532(Riot), TIA) sauf
les fichiers A2601NoFlash et A2501Flash

CREATION DE LA CARTE ROM :
	- lancer le fichier python "bin2txt.py" en précisant le chemin d'accès du fichier .a26 (Donkey Kong.a26 ici)
cela va créer un fichier text avec des valeurs exadécimales correspondant à la rom)
	- remplacer dans le fichier bench les chemin de 'fichiers Donkey Kong.txt' "audio.txt", "video.txt"
(les deux derniers fichiers seront créés par le fichier bench, definir simplement l'emplacement où ils
seront créés)

LANCEMENT DE LA SIMULATION :
	- une fois la simulation lancée et terminée, un fichier audio.txt et un fichier video.txt devraient
être créés aux emplacements spécifiés.
	- utiliser le fichier python "video.py" pour créer une image à partir du fichier "video.txt", une image
devrait apparaître. L'image que nous obtenons nous à chaque lancement est l'image "test.bmp" qui montre
une erreur.