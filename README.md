SSM
===



Introduction

L’application que nous concevrons aura pour but ultime de pouvoir faire le point sur la présence d'un employé au sein de son entreprise afin de pouvoir faire le point sur son réel planning


Architecture fonctionnelle
Cette application serait architecturée selon le design Pattern MVC. 

•	Liste des employés
Contenu dans notre base de données, elle répertoriera l’ensemble des employés travaillant au sein de notre société classés en fonction de leur département d’appartenance.
 
•	Liste des images
Ce répertoire contiendra toutes les images faciales des employés de l’entreprise classée en fonction de leur département. Pour des soucis de facilité de recherche et de rapidité, les images seront classées dans des dossiers portant le nom de chaque département. Cela permettrait donc de faciliter et d’augmenter la rapidité de la reconnaissance d’image.

•	Stockage des images dans une base de données
Stocker des images dans une base de données rendrait celle ci et son accès très lourds. Il est donc judicieux de stocker dans notre base de données leur chemins d’accès ainsi que leur nom afin d’automatiser la redirection vers le fichier contenant nos images à comparer afin d’effectuer la reconnaissance faciale.

•	Stockage dans notre bdd
Devant faire le point sur les vacances et le reste de RTT, nous devrions donc stocker cette information dans notre bdd qui sera « update » à chaque fois que besoin y aura

•	Conception du calendrier
Amener à faire le point nous devrons par employé définir l’EDT exact d’une semaine. Nous devrons donc prévoir un outil capable de générer ce calendrier grâce au check in et au check out. 




Fonctionnement
Censée être installer sur une borne aux entrées d’une entreprise, l’application fonctionne comme suit : 
1.	L’employé se pointe devant la borne puis prend ensuite une photo  à l’aide de l’application
2.	Avant ou après la prise de photo : l’employé sélectionne son département d’appartenance
3.	Si la phase deux est faite après la phase une, se lance alors la reconnaissance faciale
4.	A cette étape le check in ou check out est effectué. 
5.	(À compléter…)
