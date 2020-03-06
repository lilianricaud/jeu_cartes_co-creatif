# Règles organisation vols essaims oiseaux

Craig Reynolds a proposé 3 règles pour modéliser le comportement des vols d'oiseaux en essaim. Ces règls sont suffisantes pour simuler informatiquement avec réalisme les vols de "Boids".

1. Suivre le cap au plus près en s'orientant dans la même direction que ses congénères voisins.
2. Se tenir au milieu d'eux pour économiser de la force grace à leur protection.
3. Se tenir à distance suffisante d'eux pour ne pas les heurter, de même que d'éventuels obstacles


Comme bon nombre de simulations de vie artificielle, le programme Boids permet de modéliser un comportement émergent. En effet, la complexité comportementale résulte ici de l'interaction d'agents individuels (appelés boids) respectant un nombre limité de règles simples, telles que :

    la cohésion : pour former un groupe, les boids se rapprochent les uns des autres ;
    la séparation : 2 boids ne peuvent pas se trouver au même endroit au même moment ;
    l'alignement : pour rester groupés, les boids essayent de suivre un même chemin.

Voisinage d'un boid bidimensionnel. Du rouge le plus foncé au plus clair: zone de répulsion, d'orientation et d'attraction. La partie grise est hors du champ de vision.

Dans les faits, cela se traduit par la réaction du boid à son voisinage. Celui-ci se divise en trois zones, de la plus proche à la plus éloignée: une zone de répulsion, une zone d'orientation et une zone d'attraction. Lorsqu'un voisin entre dans la zone de répulsion, le boid s'en éloigne, s'il est dans la zone d'orientation, le boid le suit, et s'il est dans la zone d'attraction, il s'en rapproche. Généralement, on ajoute également à la simulation un angle mort, dans lequel le boid ne peut pas percevoir ses voisins. 

## source 
- Thierry Crouzet, le peuple des connecteurs, p28
Boids, Wikpédia: https://fr.wikipedia.org/wiki/Boids
