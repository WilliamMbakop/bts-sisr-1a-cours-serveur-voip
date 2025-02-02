# VoIP avec Asterisk - Théorie

## Informations

| Champ           | Détails                                |
|-----------------|---------------------------------       |
| **Auteur**      | William Mbakop                         |
| **Date**        | 13 janvier 2025                        |
| **Description** | VoIP avec Asterisk - Théorie           |

## Les notions

La VoIP (Voice over Internet Protocol) est une technologie qui permet de transmettre des appels vocaux via Internet ou d'autres réseaux IP plutôt que par les méthodes traditionnelles de communication téléphonique basées sur des lignes analogiques ou numériques. En d'autres termes, la VoIP convertit la voix en données numériques, qui sont ensuite envoyées sous forme de paquets à travers des réseaux comme Internet, permettant ainsi de passer des appels téléphoniques sur un réseau IP.

La VoIP fonctionne en convertissant le signal vocal analogique (parlant dans un téléphone) en données numériques, qui sont ensuite compressées, transmises via Internet et décodées à l'autre extrémité. Cela nécessite un équipement spécifique, comme un téléphone IP, un softphone (application logicielle pour passer des appels) ou un adaptateur VoIP pour connecter des téléphones traditionnels au réseau.

La VoIP présente plusieurs avantages : 

- Coût réduit : Les appels VoIP, surtout entre différents pays, sont souvent bien moins chers que les appels téléphoniques traditionnels.

- Flexibilité : Les utilisateurs peuvent passer des appels via Internet, ce qui permet d'utiliser la VoIP n'importe où où il y a une connexion réseau.

- Fonctionnalités supplémentaires : La VoIP offre des services tels que la messagerie vocale, la conférence audio, l'intégration avec des applications de collaboration, etc.

- Intégration avec d'autres services : Elle permet de combiner voix, vidéo et messagerie en un seul réseau de communication.

Quelques Exemples de services VoIP populaires :
- Skype
- WhatsApp
- Zoom (pour les appels vidéo et audio)
- Google Meet
- Slack (pour la communication en entreprise)

Asterisk est un logiciel open-source utilisé pour la gestion des communications VoIP (Voice over IP). Il sert de plateforme de PBX (Private Branch Exchange), permettant la gestion des appels vocaux sur des réseaux IP. Asterisk permet de configurer des fonctionnalités telles que la gestion des appels entrants et sortants, la messagerie vocale, les conférences téléphoniques, la gestion des annuaires, et l'intégration avec d'autres services.


## Architecture


L'architecture typique consiste en un serveur central sur lequel Asterisk est installé et des machines clientes équipées de Softphones, comme 3CX. 

Asterisk, en tant que serveur de communication, gère les appels vocaux et assure la connectivité entre les différentes extensions et réseaux téléphoniques. 

Les clients, qui utilisent le Softphone 3CX, sont des applications installées sur des ordinateurs, smartphones ou tablettes. Ces softphones se connectent au serveur Asterisk **via le protocole SIP** (Session Initiation Protocol) ou un autre protocole de VoIP pour passer et recevoir des appels. 

Asterisk gère la signalisation, la gestion des appels, les fonctionnalités avancées (comme la messagerie vocale ou les conférences), et s'assure de la qualité et de la fiabilité des communications entre les clients, tout en étant compatible avec des protocoles standards de VoIP.

3CX, en tant que Softphone, permet aux utilisateurs d'avoir une interface simple et intuitive pour gérer leurs appels, tout en étant entièrement compatible avec le serveur Asterisk.

## Ports utilisés : 

Les ports couramment utilisés dans le cadre de la VoIP sont :

- **SIP (Session Initiation Protocol)** : Utilise généralement les ports 5060 (non sécurisé) et 5061 (sécurisé avec TLS).
- **RTP (Real-time Transport Protocol)** : Utilise une plage de ports UDP, souvent entre 10000 et 20000, pour le transport des flux audio et vidéo.
- **IAX (Inter-Asterisk eXchange)** : Utilise le port 4569 pour la communication entre serveurs Asterisk.

Ces ports peuvent varier en fonction de la configuration spécifique du système VoIP.

## Liens utiles :

- https://www.asterisk.org/
- https://www.youtube.com/watch?v=vqqEcDC972c&list=PL3GzJ6OC0xVjvz7me4YvPUumYKVkiZSfZ&index=5