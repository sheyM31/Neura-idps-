# 🧠 Neura-IDPS

Neura-IDPS est un système intelligent de détection et de prévention des intrusions (IDPS) combinant :
- surveillance réseau
- analyse des interactions avec les modèles d’IA
- intelligence artificielle (Machine Learning)
- moteur de décision autonome (Hestia)

---

## 🏗️ Architecture Fonctionnelle

### 🔹 Sources de données
- 🌐 Trafic réseau
- 🤖 Échanges utilisateur ↔ système IA

---

## 📡 Capteurs

Deux types de capteurs :

### 1. Capteurs réseau
- Collecte des métadonnées des paquets
- Analyse du trafic

### 2. Capteurs IA
- Entrées utilisateur (prompts)
- Sorties du modèle (réponses IA)
- Décryptage si nécessaire

## le module core

 
core orchestre le fonctionnement du système.assure la communication entre module.
il récupère les résultats de l'analyse des modèles IA et les Envois à hestia

## AI modèles

analyse les métadonnées des paquets et les échanges utilisateur/IA pour détecter les anomalies

## hestia

module d'action du système
il est doté d'un analyseur de score de confiance et d'un sous module de décision qui décide des actions à appliquer

---

##  Pipeline de traitement

```text
[ Capteurs ]
      ↓
[ Vérification des règles ]
      ↓
 ┌───────────────┬───────────────┐
 │               │               │
❌ Non conforme   ✅ Conforme
 │               ↓
 ↓       [ Modèles IA ]
[ Hestia ]        ↓
 (blocage)   [ Scores de confiance ]
                  ↓
            [ Analyseur de score ]
                  ↓
            [ Module de décision ]

## comment lancé 