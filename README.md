# La Terre vue de nuit - TerraGazer

Dans le monde, 1 personne sur 10 n'a pas accès à l'électricité. Afin de pouvoir apporter de l'aide à ces personnes, il est nécessaire d'avoir des données de recensement précises et à jour. Cependant, de telles données sont rares dans les pays défavorisés. Nous nous concentrerons sur la région du Sokoto, Nigeria.

Nous cherchons donc à générer des données équivalentes en utilisant une approche basée sur le Machine Learning, et l'abondance de données satellites librement accessibles capturées en continu. Nous nous intéressons particulièrement à des images de nuit capturant la luminosité ambiante au sol, en les utilisant comme proxy de présence humaine.

Une fois correctement traitées et préparées, ces données servent à entraîner un réseau de neurones convolutionnel prédisant la luminosité émise par différents emplacements. Le résultat souhaité prend la forme des zones habitées prédites comme émettant de la lumière par le modèle, mais n'émettant en réalité  aucune lumière. Ces emplacements sont les villages défavorisés que l'on cherche à détecter.

## Installation

Ce repository GitHub a été mis en place afin de pouvoir reproduire les résultats obtenus au cours de ce projet et donne accès à l'intégralité des fichiers nécessaires. 

Pour pouvoir exécuter chacun des notebooks, un environnement ```conda``` est recommandé. Il est aussi nécessaire d'installer ```pip```. Le script ```newenv.sh``` permet d'installer l'ensemble des librairies python nécessaires, à travers ```pip``` ainsi que ```conda```. Il est aussi techniquement possible d'installer les prérequis grâce à la commande ```pip install -r requirements.txt```. Cependant, des erreurs peuvent être engendrées à cause des paquets uniquement disponibles sur conda. 

Attentions aux utilisateur n'utilisant pas Windows: Le paquet ```pywin32``` inclut dans le script et les requirements, est nécessaire et exclusif à Windows, et doit être désactivé avant de poursuivre sur d'autres systèmes d'exploitation.

Une fois les paquets installés, les notebooks peuvent être lancés grâce à la commande ```jupyter-lab```. Les notebooks sont numérotés dans l'ordre logique de leur exécution au cours du projet afin de recréer les résultats obtenus.