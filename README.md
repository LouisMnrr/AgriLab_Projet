<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projet Serre Connectée</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .nav {
            background-color: #8BC34A; /* Vert clair */
            color: white;
            padding: 10px;
            text-align: center;
        }
        .nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
        }
        .nav a:hover {
            text-decoration: underline;
        }
        .page {
            display: none;
            padding: 20px;
        }
        .page.active {
            display: block;
        }
        .cover-page h1 {
            font-size: 2.5em;
            margin-bottom: 0.5em;
        }
        .cover-page p {
            font-size: 1.2em;
            margin-top: 0;
        }
        .cover-page img {
            max-width: 100%;
            height: auto;
            margin-top: 20px;
        }
        .week-section {
            margin-bottom: 40px;
        }
        .week-section h2 {
            border-bottom: 2px solid #8BC34A; /* Vert clair */
            padding-bottom: 10px;
            font-weight: bold;
        }
        .actions {
            padding-left: 20px;
        }
        .actions li {
            margin-bottom: 5px;
        }
        .bold {
            font-weight: bold;
        }
        #google_translate_element {
            margin-top: 20px;
            text-align: center;
        }
        .custom-image {
            width: 300px;
            height: auto; /* Maintient le ratio de l'image */
        }
    </style>
    <script src="https://translate.google.com/translate_a/element.js?cb=googleTranslateElementInit"></script>
    <script>
        function showPage(pageId) {
            const pages = document.querySelectorAll('.page');
            pages.forEach(page => page.classList.remove('active'));
            document.getElementById(pageId).classList.add('active');
        }

        function googleTranslateElementInit() {
            new google.translate.TranslateElement({pageLanguage: 'fr'}, 'google_translate_element');
        }
    </script>
</head>
<body>
    <div class="nav">
        <a href="#" onclick="showPage('cover-page')">Page de Garde</a>
        <a href="#" onclick="showPage('documentation-page')">Documentation</a>
        <a href="#" onclick="showPage('sources-page')">Sources</a>
    </div>
    
    <div id="cover-page" class="cover-page page active">
        <h1>Projet Serre Connectée</h1>
        <p>Document de suivi et de gestion du projet</p>
        <p>Date de début : [2023-2024]</p>
        <p>Étudiants responsables du projet : Louis Monnier / Jules Boursiez / Augustin Cailliez</p>
        <p>Responsable du projet : Nicolas Kaufmann</p>
        <img src="AgriLab/Beauvais_Fermes.jpg" alt="Image de la serre connectée">
        <div id="google_translate_element"></div>
    </div>
    
    <div id="documentation-page" class="documentation-page page">
        <h1>Documentation</h1>
        <div class="week-section">
            <h2>Semaine 1</h2>
            <ul class="actions">
                <li>
                    <span class="bold">MATÉRIAUX & USTENSILES pour le projet :</span>
                    <p> Action n° 1 : Relevé des décisions des matériaux </p>
                    <ul>
                        <li>1. <span class="bold">Arduino Uno R3 :</span> Ce microcontrôleur est utilisé pour programmer et contrôler les capteurs et les actionneurs dans un projet. Il sert de cerveau au système, permettant la lecture des données des capteurs et le contrôle des composants actifs comme les moteurs ou les LEDs.</li>
                        <li>2. <span class="bold">Capteur flotteur :</span> Ce capteur détecte le niveau de liquide dans un réservoir. Il envoie un signal à l'Arduino pour indiquer si le niveau du liquide est trop bas ou trop haut, ce qui peut déclencher des actions comme allumer une pompe ou une alarme.</li>
                        <li>3. <span class="bold">Presse étoupe :</span> Dispositif d'étanchéité utilisé pour passer un câble à travers une paroi tout en maintenant l'étanchéité et en protégeant le câble contre l'usure et les dommages, essentiel pour les installations où l'étanchéité est cruciale.</li>
                        <li>4. <span class="bold">Boîtier PVC :</span> Enclosure qui protège l'électronique, comme l'Arduino et les autres composants, des éléments extérieurs tels que l'eau, la poussière et les impacts physiques, assurant ainsi leur longévité et leur bon fonctionnement.</li>
                        <li>5. <span class="bold">Câble Arduino :</span> Ce câble, généralement un câble USB, permet de connecter l'Arduino à un ordinateur pour la programmation ou à une alimentation externe pour fournir l'énergie nécessaire à son fonctionnement.</li>
                        <li>6. <span class="bold">Câble alimentation 3 brins :</span> Câble électrique robuste utilisé pour fournir l'alimentation aux composants nécessitant une alimentation plus forte, comme des pompes ou des moteurs, assurant une distribution stable et sécurisée de l'électricité.</li>
                        <li>7. <span class="bold">Polycarbonate 3 mm :</span> Matériau solide et transparent utilisé pour fabriquer des protections ou des supports pour les composants électroniques. Le polycarbonate est résistant aux impacts et aux conditions extérieures, idéal pour les environnements exigeants.</li>
                        <li>8. <span class="bold">Tuyau PVC :</span> Tuyau utilisé pour transporter des liquides. Le PVC est résistant à la corrosion, durable et capable de supporter une pression élevée, ce qui en fait un choix idéal pour diverses applications de plomberie et de transfert de liquide.</li>
                        <li>9. <span class="bold">Tuyau goutte à goutte :</span> Tuyau spécialement conçu pour l'irrigation, permettant la distribution de l'eau en petites quantités directement aux racines des plantes, ce qui économise l'eau et assure une irrigation efficace.</li>
                        <li>10. <span class="bold">Colle PVC :</span> Adhésif utilisé pour assembler les composants en PVC, garantissant une connexion solide et étanche entre les pièces, essentielle pour maintenir l'intégrité des systèmes de tuyauterie.</li>
                        <li>11. <span class="bold">Connecteur et raccord :</span> Dispositifs utilisés pour connecter différentes sections de tuyaux ou pour relier les tuyaux à d'autres composants comme des valves ou des pompes, assurant une transition fluide et sécurisée des liquides ou des gaz.</li>
                        <li>12. <span class="bold">Valve :</span> Dispositif utilisé pour contrôler le débit de liquide à travers un tuyau. Il peut être actionné manuellement ou via un actionneur, permettant de réguler ou d'arrêter le flux selon les besoins du système.</li>
                        <li>13. <span class="bold">Serre-câble :</span> Dispositif utilisé pour fixer et organiser les câbles, empêchant les enchevêtrements et les dommages, tout en maintenant une installation propre et sécurisée.</li>
                        <li>14. <span class="bold">Pompe à liquide péristaltique :</span> Pompe utilisée pour déplacer des liquides de manière précise et contrôlée. Elle fonctionne en compressant et en relâchant un tuyau flexible, idéale pour des applications nécessitant une manipulation hygiénique et précise des liquides.</li>
                        <li>15. <span class="bold">Shield Ethernet :</span> Extension pour l'Arduino permettant la connectivité réseau, ce qui permet à l'Arduino de communiquer via Internet ou un réseau local, ouvrant des possibilités pour la surveillance à distance et le contrôle des systèmes.</li>
                    </ul>
                    <p>Comparaison des composants similaires ou redondants :</p>
                    <ul>
                        <li><span class="bold">Tuyau PVC vs. Tuyau goutte à goutte :</span>
                            <ul>
                                <li><span class="bold">Tuyau PVC :</span> Utilisé pour des applications générales de transport de liquide avec une résistance mécanique élevée.</li>
                                <li><span class="bold">Tuyau goutte à goutte :</span> Spécifiquement conçu pour l'irrigation avec un débit d'eau contrôlé.</li>
                                <li><span class="bold">Résultat :</span> Utilisation complémentaire des deux types pour optimiser le système d'irrigation.</li>
                            </ul>
                        </li>
                        <li><span class="bold">Capteur flotteur vs. Valve :</span>
                            <ul>
                                <li><span class="bold">Capteur flotteur :</span> Détecte le niveau de liquide.</li>
                                <li><span class="bold">Valve :</span> Contrôle le flux de liquide.</li>
                                <li><span class="bold">Résultat :</span> Intégration des deux pour une gestion précise du niveau et du débit de liquide.</li>
                            </ul>
                        </li>
                    </ul>
                </li>
            </ul>
        </div>
        <div class="week-section">
            <h2>Semaine 2</h2>
            <ul class="actions">
                <li><span class="bold">Action n° 1 :</span> Fabrication de la serre en polycarbonate 3mm avec l'aide du FabLab et découpeuse laser.</li>
                <li><span class="bold">Action n° 2 :</span> Installation de la pompe péristaltique, test du débit et de la gestion via l'Arduino.</li>
            </ul>
        </div>
        <div class="week-section">
            <h2>Semaine 3</h2>
            <ul class="actions">
                <li><span class="bold">Action n° 1 :</span> Réalisation du programme pour l'ESP8266 pour connecter la serre à Internet et permettre le contrôle à distance.</li>
                <li><span class="bold">Action n° 2 :</span> Intégration des capteurs et test de la communication avec l'ESP8266.</li>
            </ul>
        </div>
        <div class="week-section">
            <h2>Programme ESP8266</h2>
            <pre>
                <code>
#include &lt;ESP8266WiFi.h&gt;
#include &lt;PubSubClient.h&gt;

// Réglages WiFi
const char* ssid = "votre_SSID";
const char* password = "votre_mot_de_passe";

// Réglages MQTT
const char* mqtt_server = "adresse_du_serveur_MQTT";
const int mqtt_port = 1883;
const char* mqtt_user = "votre_utilisateur";
const char* mqtt_password = "votre_mot_de_passe";

// Création des objets WiFi et MQTT
WiFiClient espClient;
PubSubClient client(espClient);

void setup() {
  Serial.begin(115200);
  setup_wifi();
  client.setServer(mqtt_server, mqtt_port);
  client.setCallback(callback);
}

void setup_wifi() {
  delay(10);
  // Connexion au WiFi
  Serial.println();
  Serial.print("Connexion à ");
  Serial.println(ssid);
  WiFi.begin(ssid, password);

  while (WiFi.status() != WL_CONNECTED) {
    delay(500);
    Serial.print(".");
  }

  Serial.println("");
  Serial.println("WiFi connecté");
  Serial.println("Adresse IP : ");
  Serial.println(WiFi.localIP());
}

void callback(char* topic, byte* payload, unsigned int length) {
  Serial.print("Message reçu [");
  Serial.print(topic);
  Serial.print("] ");
  for (int i = 0; i < length; i++) {
    Serial.print((char)payload[i]);
  }
  Serial.println();
}

void reconnect() {
  while (!client.connected()) {
    Serial.print("Tentative de connexion MQTT...");
    if (client.connect("ESP8266Client", mqtt_user, mqtt_password)) {
      Serial.println("connecté");
      client.subscribe("inTopic");
    } else {
      Serial.print("échec, rc=");
      Serial.print(client.state());
      Serial.println(" nouvelle tentative dans 5 secondes");
      delay(5000);
    }
  }
}

void loop() {
  if (!client.connected()) {
    reconnect();
  }
  client.loop();
}
                </code>
            </pre>
            <p>Ce programme permet de connecter l'ESP8266 à un réseau WiFi et de communiquer avec un serveur MQTT. Les principales étapes sont :</p>
            <ul>
                <li>Connexion au réseau WiFi spécifié par les constantes <code>ssid</code> et <code>password</code>.</li>
                <li>Connexion au serveur MQTT avec les identifiants définis.</li>
                <li>Publication et souscription à des topics pour envoyer et recevoir des messages MQTT.</li>
                <li>Reconnexion automatique en cas de déconnexion du serveur MQTT.</li>
            </ul>
            <p>Ce programme est essentiel pour permettre la surveillance et le contrôle à distance de la serre connectée via Internet.</p>
        </div>
    </div>

    <div id="sources-page" class="sources-page page">
        <h1>Sources</h1>
        <p>Les ressources et informations suivantes ont été utilisées pour réaliser ce projet :</p>
        <ul>
            <li>Documentation officielle Arduino</li>
            <li>Documentation officielle ESP8266</li>
            <li>Manuels et guides des fabricants des capteurs et composants utilisés</li>
            <li>Tutoriels et exemples de projets similaires disponibles en ligne</li>
        </ul>
    </div>
</body>
</html>
