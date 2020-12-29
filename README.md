# OpenSignalFr

Dispositif de signalement électronique ou numérique Open Source intégration BetaFlight esp32


Qu’est-ce qu’un dispositif de signalement électronique ou numérique ?
Il s’agit d’un dispositif à bord de l’aéronef qui émet un signalement wifi. Ce signalement est diffusé à tout.
Instant du vol, et contient un identifiant unique et des informations relatives au vol : position de l’aéronef,
Position du point de décollage, vitesse sol et route suivie.


Pourquoi ?
Une seule marque présente sur le marché &amp; dispositif très cher &gt; 149 (pour une puce GPS et wifi)
Les racers sont souvent déjà équipés de GPS =&gt; inutile d'en porter deux.

Proofs of concept.
J'ai commandé des esp32 et esp8266 de plusieurs modèles.
Pistes de modèles(besoin d'un régulateur 5v) et plus petit possible :
-
-
-

Pour l'instant, je pense que le fonctionnement va marcher comme ceci:

Gps(ex bn-180) =Serial=&gt; Fc betaflight =Telemetry Rx=&gt; Module wifi(esp32, esp8266)

Dans un premier temps le module sera programmé avec un bootloader arduino, ensuite je souhaiterais créer un utilitaire plus accessible.
Le numéro d'identification sera flashé en même temps que le programme.

Conclusion :
Moins cher, moins lourds que les dispositifs déjà vendus.
