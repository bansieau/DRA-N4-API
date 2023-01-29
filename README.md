# DRA-N4-API
DENON Ceol Piccolo (DRA-N4) API Informations

La Ceol Piccolo (DRA-N4) est une station HiFi domestique réseau de chez DENON. Elle posséde une API non documentée (probablement utilisée par l'application mobile) qui permet sa commande via le réseau. Ce dépot concentre mes recherches de documentation et de rétro-ingiénérie sur le sujet.

## Accéder à l'API
On fait un appel à l'API avec : http://**[Adresse IP]**/goform/formiPhoneAppDirect.xml?**[Commande]**

Les commandes (actuellement trouvée) sont les suivantes :

* Alimentation
  * **PWON** - Allumer l'appareil
  * **PWSTANDBY** - Mettre en veille l'appareil
* Sélection de l'entrée
  * **SIRADIO** - Radio internet
  * **SISERVER** - Serveur DLNA
  * **SIANALOGIN** - Entrée analogique
  * **SIDIGITALIN1** - Entrée numérique
  * **SIUSB** - Entrée USB/Ipod
* Volume
  * **MVUP** - Augementer le volume
  * **MVDOWN** - Baisser le volume
  * **MUON** - Activer le mode muet
  * **MUOFF** - Déactiver le mode muet
  * **MV00**/**MV60** - Définir le niveau de volume de 00 à 60 (toujours indiquer deux chiffres)
* Veille programmée (Sleep)
  * **SLPOFF** - Déactiver la veille programmée
  * **SLP001** / **SLP120** - Définir le délais avant mise en veille programmée de 001 à 120 minutes (toujours indiquer trois chiffres)
