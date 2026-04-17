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
