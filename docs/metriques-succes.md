## Métriques de Succès — GROUPE BUSINESS

### MVP
Plateforme mobile GalleExpress permettant à un prestataire informel de Dakar de créer un profil vérifié, de recevoir des demandes de clients et d'être contacté directement — le tout sans intermédiaire, depuis un smartphone Android, avec paiement via Wave.

---

### ⭐ Métrique Nord
**Indicateur :** Nombre de mises en relation ayant abouti à une mission réellement effectuée et confirmée par les deux parties (prestataire + client) sur GalleExpress

**Valeur cible à 30 jours :** 10 missions complétées et confirmées

**Comment mesurer :** Appel téléphonique ou message WhatsApp de suivi envoyé par Rokhaya (Responsable Impact) à chaque prestataire ayant reçu une demande — cocher "mission effectuée : oui/non" dans un tableau Google Sheets partagé avec l'équipe

---

### 📈 Métriques de Progression

#### Métrique P1
**Indicateur :** Nombre de prestataires ayant créé un profil complet et vérifié sur GalleExpress (photo + spécialité + quartier + numéro Wave renseignés)

**Valeur cible à 30 jours :** 20 profils prestataires actifs et complets

**Comment mesurer :** Comptage manuel hebdomadaire dans la base de données GalleExpress — un profil est "complet" uniquement si les 4 champs obligatoires sont renseignés ; Elhadji Omar Diallo vérifie chaque nouveau profil avant activation

---

#### Métrique P2
**Indicateur :** Nombre de demandes de services publiées par des clients sur la plateforme en 30 jours

**Valeur cible à 30 jours :** 25 demandes publiées

**Comment mesurer :** Comptage direct dans le tableau de bord GalleExpress ou dans le Google Sheets de suivi — Fatima consolide le nombre chaque lundi matin et note la catégorie de service (plomberie, électricité, etc.) pour identifier les secteurs les plus actifs

---

#### Métrique P3
**Indicateur :** Taux de complétion du flux d'inscription prestataire — proportion de prestataires ayant commencé l'inscription et l'ayant terminée sans abandon

**Valeur cible à 30 jours :** 70% des prestataires ayant démarré l'inscription finalisent leur profil

**Comment mesurer :** Comparer le nombre de profils "initiés" (étape 1 validée) au nombre de profils "complets" (4 champs renseignés) dans le suivi hebdomadaire — un écart supérieur à 30% déclenche une investigation terrain immédiate

---

### 🚨 Métriques d'Alerte

#### Alerte A1 — Désintermédiation vers WhatsApp
**Signal :** Proportion de mises en relation où le client et le prestataire ont échangé leurs contacts personnels et finalisé la mission hors de GalleExpress, sans confirmation sur la plateforme

**Seuil :** Plus de 40% des mises en relation ne donnent lieu à aucune confirmation de mission sur GalleExpress dans les 72h suivant le premier contact

**Action corrective :** Organiser immédiatement 3 entretiens courts avec des prestataires concernés pour identifier ce qui manque sur la plateforme (garantie, paiement sécurisé, historique) — puis ajouter en urgence la fonctionnalité de valeur manquante avant la démo S6

---

#### Alerte A2 — Abandon à l'inscription
**Signal :** Taux d'abandon du flux d'inscription prestataire supérieur au seuil acceptable — trop de prestataires commencent mais ne terminent pas leur profil

**Seuil :** Moins de 50% des prestataires ayant démarré l'inscription finalisent leur profil en moins de 15 minutes

**Action corrective :** Conduire un test utilisateur d'urgence avec 2 prestataires réels en observation silencieuse — identifier le champ ou l'étape qui bloque, simplifier ou supprimer immédiatement l'obstacle identifié

---

### Tableau de Bord S6
À la démo S6, nous présenterons ces 3 chiffres :
1. **Métrique Nord** — Missions complétées et confirmées : X réel sur 10 cibles
2. **Métrique P1** — Profils prestataires actifs et complets : X réel sur 20 cibles
3. **Alerte A1** — Désintermédiation vers WhatsApp : déclenchée (>40%) ou non (<40%)
