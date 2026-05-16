# 🛡️ FUTURE_CS_01 — Tâche 1 Cybersécurité

## 📌 Présentation du projet

Ce dépôt contient le travail réalisé dans le cadre de la **Tâche 1 du programme de stage en cybersécurité de Future Interns (2026)**.

L’objectif de cette mission est d’effectuer une **analyse de vulnérabilités en lecture seule** sur un site web public, puis de documenter les résultats sous forme de rapport professionnel.

---

## 🎯 Objectif de la mission

Les objectifs principaux sont :

- Analyser un site web public afin d’identifier des failles de sécurité courantes
- Identifier les services exposés et configurations faibles
- Vérifier les en-têtes de sécurité HTTP
- Classer les risques (Faible / Moyen / Élevé)
- Proposer des recommandations de correction claires et compréhensibles
- Présenter les résultats dans un format professionnel

---

## 🌐 Site analysé

- **Site testé :** OWASP Juice Shop (environnement de démonstration)
- **URL :** https://demo.owasp-juice.shop  
- **Type d’analyse :** Lecture seule / analyse passive
- **Règles respectées :** aucune attaque, aucun contournement, aucune exploitation

---

## 🛠️ Outils utilisés

- **Nmap** → Analyse des ports et services exposés
- **OWASP ZAP (mode passif)** → Analyse des vulnérabilités web
- **DevTools navigateur** → Inspection des en-têtes HTTP et cookies
- **Kali Linux** → Environnement de test

---

## 📊 Méthodologie

1. Scan du site avec Nmap pour identifier les ports ouverts
2. Analyse des services et technologies exposées
3. Vérification des en-têtes HTTP de sécurité
4. Analyse passive avec OWASP ZAP
5. Collecte des résultats et documentation
6. Classification des risques et recommandations

---

## 🔍 Principales observations

Les éléments suivants ont été identifiés :

- Services réseau exposés (FTP, HTTP, DNS, etc.)
- Configuration faible de certains en-têtes de sécurité
- Exposition d’informations serveur dans les réponses HTTP
- Présence d’un proxy / load balancer (F5 BIG-IP)
- Politiques de sécurité HTTP incomplètes

---

## ⚠️ Classification des risques

- 🔴 **Risque élevé** : Services exposés pouvant augmenter la surface d’attaque
- 🟠 **Risque moyen** : Mauvaises configurations de sécurité
- 🟢 **Risque faible** : Informations non critiques ou informatives

---

## 📁 Structure du dépôt

FUTURE_CS_01/
├── README.md
├── evidence/
├── screenshots/
├── notes/
├── report/
└── tools/


---

## 📄 Livrables

✔ Rapport d’évaluation des vulnérabilités (PDF Canva)  
✔ Résultats du scan Nmap  
✔ Résultats OWASP ZAP (analyse passive)  
✔ Captures d’écran des outils  
✔ Dépôt GitHub structuré et documenté  

---

## 📌 Compétences développées

- Analyse de vulnérabilités web
- Compréhension des risques réseau
- Lecture et interprétation des en-têtes HTTP
- Classification des risques en cybersécurité
- Rédaction d’un rapport de sécurité professionnel

---

## 🚀 Conclusion

Cette mission permet de comprendre les bases de l’audit de sécurité web dans un contexte professionnel.

Elle met l’accent sur l’analyse, la documentation et la communication des risques, plutôt que sur l’exploitation technique.

---

## 🔗 Programme de stage

**Future Interns — Parcours Cybersécurité 2026**  
#futureinterns

---

## 👤 Auteur

Stagiaire en cybersécurité : ADOGNON Komlan Dosseh Aimé 
Programme : Future Interns (2026)
