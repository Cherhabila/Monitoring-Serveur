# Monitoring-Serveur 🚀

Système complet de supervision, de métrologie et d'alerting automatisé basé sur la stack open-source **Prometheus**, **Grafana** et **Alertmanager**.

## 🏗️ Architecture & Composants
Ce projet centralise la collecte des indicateurs de performance de plusieurs machines cibles en temps réel :
* **Prometheus** : Serveur central de collecte et base de données orientée séries temporelles.
* **Grafana** : Interface de visualisation avancée avec tableaux de bord dynamiques (*Node Exporter Full*).
* **Alertmanager** : Moteur de gestion et d'aiguillage des alertes système.

## 🖥️ Cibles Supervisées (Targets)
Le cluster de monitoring remonte actuellement les métriques système de 3 nœuds d'infrastructure :
1. **Ser-test** (Serveur principal accueillant la stack)
2. **Node1** (Nœud d'infrastructure distant)
3. **Node2** (Nœud d'infrastructure distant)

## 🛠️ Déploiement Rapide
Pour instancier l'infrastructure de monitoring complète via Docker Compose :
```bash
docker compose up -d
