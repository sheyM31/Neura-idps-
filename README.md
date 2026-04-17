🧠 Neura-IDPS

Neura-IDPS est un système intelligent de détection et de prévention d’intrusions (IDPS) basé sur l’intelligence artificielle.
Il combine l’analyse du trafic réseau,la surveillance des échanges utilisateur/IA, le machine learning et un moteur de décision autonome pour détecter et réagir aux comportements suspects en temps réel.


---

🚀 Vision du projet

Créer un système de cybersécurité intelligent capable de :

détecter les attaques réseau en temps réel

protéger les systèmes d'intelligence artificielle contre les attaques adversarial

analyser les comportements anormaux via ML

prendre des décisions autonomes (alerte, blocage, mitigation)

évoluer avec de nouvelles données d’attaques



---

🏗️ Architecture globale

[ Sensors ]
   ↓
[ Core Engine ]
   ↓
[ ML Models ]
   ↓
[ Hestia Decision Engine ]
   ↓
[ Actions (Alert / Block / Log) ]


---

🧩 Structure du projet

Neura-IDPS/
│
├── core/              # Orchestrateur principal du système
├── sensors/           # Collecte des données (réseau,prompt utilisateur/sortie du model)
├── models/            # Modèles ML (Isolation Forest, Random Forest)
├── hestia/            # Moteur de décision et réponse
├── training/          # Scripts d'entraînement des modèles
├── data/              # Datasets
(CICIDS2018)
├── utils/             # Fonctions utilitaires
├── logs/              # Logs du système
└── README.md


---

🤖 Intelligence artificielle

Neura-IDPS utilise des algorithmes de machine learning pour la détection d’anomalies :

Isolation Forest → détection d’anomalies non supervisée

Random Forest → classification des attaques connues

Feature Engineering → transformation des données réseau


Pipeline ML :

Data → Preprocessing → Feature Extraction → Training → Prediction → Decision


---

⚙️ Fonctionnement

1. Les sensors capturent les données réseau


2. Le core centralise et normalise les événements


3. Les modèles ML analysent et détectent les anomalies


4. Hestia prend une décision (autoriser / bloquer / alerter)


5. Le système exécute l’action en temps réel




---

📊 Dataset utilisé

CICIDS2018 (principal)

Possibilité d’ajouter d’autres datasets IDS/IPS



---

🛠️ Installation

git clone https://github.com/sheyM31/Neura-idps-
cd Neura-idps-

pip install -r requirements.txt


---

▶️ Lancement 

python core/main.py


---

🧪 Objectifs futurs

intégration deep learning (LSTM / Transformer)

dashboard de monitoring en temps réel

système d’auto-adaptation des modèles

déploiement en environnement réseau réel

API de sécurité pour intégration externe



---

⚠️ Avertissement

Ce projet est en développement.
Les modèles et décisions doivent être testés avant utilisation en production.


---

👤 Auteur

Projet développé par neura labs
Orientation : cybersécurité + intelligence artificielle


---

🔥 Résumé

Neura-IDPS vise à devenir un système de défense autonome intelligent, capable de comprendre et réagir aux menaces réseau et aux attaques adversarial sans intervention humaine constante.

