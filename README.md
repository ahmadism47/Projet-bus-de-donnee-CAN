# Projet-bus-de-donnee-CAN

L’objectif est de récupérer sur le PC Host les informations de différents capteurs.
Toutes les informations vont transiter sur un bus de terrain, le bus CAN.

Les capteurs ne pouvant émettre directement sur ce Bus, des microcontrôleurs ST-Nucleo récupèrent la valeur du capteur pour la placer dans les trames CAN.

Une première carte permet de contrôler un servomoteur robotis dynamixel ; elle permet également la mesure de la vitesse du vent(anémomètre SOMFY)

Une deuxième carte µC récupère une donnée de luminosité ou de distance via un bus I2C (Capteur ST VL6180X), ainsi que des données de pression et d’humidité ( Capteurs ST LPS22HB et HTS221 ).

Une troisième carte µC récupère les données d’un accéléromètre et d’un gyroscope via un bus I2C (Capteur Invensense MPU9250)

![My Photo](architecture.svg)
