# tp2_Java_Boudaoudi_ARIBA
L'objectif de cette seconde partie était de passer du traitement de données (Backend) à la visualisation graphique (Frontend). Nous avons utilisé la bibliothèque JavaFX pour créer un environnement 3D interactif représentant le globe terrestre et le trafic aérien.
# 1. La Modélisation de la Terre (Earth.java)

Ce qu'on a fait :

Nous avons créé une classe Earth qui hérite de javafx.scene.Group. Cela permet de manipuler la Terre et tous les objets qui y sont collés (aéroports) comme un seul bloc.

Points techniques à expliquer :

La Sphère : Utilisation de l'objet Sphere de JavaFX avec un rayon de 300 unités.

La Texture (Mapping) : Pour que la sphère ressemble à la Terre, nous avons utilisé un PhongMaterial. C'est un matériau qui gère la lumière et la texture. Nous avons appliqué l'image image_ad4b04.jpg comme DiffuseMap. Cela "emballe" l'image autour de la sphère.

L'optimisation : La classe Earth stocke la sphère principale mais aussi toutes les petites sphères rouges. En héritant de Group, si on fait tourner l'objet Earth, tout tourne en même temps (la planète et les aéroports).

<img width="599" height="473" alt="image" src="https://github.com/user-attachments/assets/f3eeda5d-d16e-42a4-b84d-3f7a0043c9fb" />

