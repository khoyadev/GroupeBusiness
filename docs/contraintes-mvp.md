Contraintes MVP — Groupe Business
Persona
•	Nom : Mamadou Diop, 32 ans, plombier indépendant
•	Localisation : Dakar, Sénégal
•	Activité : Prestataire de services à domicile
•	Frictions : Difficulté à trouver des clients réguliers, manque de visibilité, concurrence importante
•	Équipement : Smartphone Android, compte Wave
________________________________________
Contraintes Non Négociables
Contrainte 1
Critère : Le MVP DOIT fonctionner sur un smartphone Android d'entrée de gamme avec une connexion data limitée (3G), avec des pages dont le poids n'excède pas 200 Ko et une interface utilisable sans compte Google actif.
Origine : Chapeau Blanc (taux de pénétration smartphone >50% en urbain, ARTP 2023) + Chapeau Noir (risque de fracture numérique fonctionnelle)
Élimine : Toute interface construite avec des frameworks lourds (animations complexes, images haute résolution, chargement de cartes en temps réel), les fonctionnalités vidéo de présentation de profil, et les dashboards avec graphiques dynamiques.
________________________________________
Contrainte 2
Critère : Le MVP DOIT intégrer Wave comme seul moyen de paiement natif et NE DOIT PAS proposer de carte bancaire ou virement bancaire comme option principale.
Origine : Chapeau Blanc (adoption massive de Wave à Dakar, cohérence culturelle confirmée)
Élimine : L'intégration Stripe, PayPal ou tout système de paiement par carte — ces options ne correspondent pas aux habitudes financières de Mamadou ni de sa clientèle cible à Dakar.
________________________________________
Contrainte 3
Critère : Le MVP DOIT maintenir une valeur ajoutée exclusive post-mise en relation (historique vérifié, système d'évaluation, garantie de transaction) afin que quitter la plateforme pour WhatsApp représente une perte réelle pour les deux parties.
Origine : Chapeau Noir (risque de désintermédiation rapide vers WhatsApp)
Élimine : Une messagerie interne basique sans différenciation — un simple chat sans historique certifié ni lien avec les évaluations n'offre aucune raison de rester sur la plateforme plutôt que de basculer sur WhatsApp.
________________________________________
Contrainte 4
Critère : Le MVP DOIT inclure un mécanisme minimal de vérification d'identité à l'inscription (numéro de téléphone Wave vérifié + photo de profil obligatoire) et NE DOIT PAS autoriser de profil prestataire anonyme ou incomplet à apparaître dans les résultats de recherche.
Origine : Chapeau Noir (risque de faux profils et d'arnaque détruisant la confiance)
Élimine : L'inscription en un clic sans vérification, les profils sans photo, et la publication immédiate sans validation minimale — ces approches "frictionless" sont incompatibles avec la promesse de confiance qui est le cœur du projet.
________________________________________
Contrainte 5
Critère : Le MVP DOIT permettre la création d'un profil prestataire complet en moins de 5 minutes, avec des champs courts, des listes déroulantes prédéfinies (catégorie de service, quartier) et une option de description vocale ou par emoji.
Origine : Chapeau Noir (risque de fracture numérique fonctionnelle) + Chapeau Blanc (97% emploi informel, BIT 2020 — majorité sans présence numérique ni habitude de formulaires)
Élimine : Les formulaires longs à saisie libre, les champs CV ou portfolio PDF, et toute étape d'inscription qui suppose une aisance rédactionnelle en français formel.
________________________________________
Fonctionnalités Éliminées
•	Système de recommandation algorithmique (matching IA) → éliminé parce que la Contrainte 1 interdit les interfaces lourdes et que l'IA nécessite des volumes de données inexistants au stade MVP.
•	Paiement par carte bancaire ou virement SEPA → éliminé parce que la Contrainte 2 impose Wave comme seul levier de paiement cohérent avec le contexte utilisateur.
•	Chat interne sans valeur ajoutée certifiée → éliminé parce que la Contrainte 3 exige que la messagerie soit liée aux évaluations et à l'historique — sans quoi elle ne retient pas les utilisateurs face à WhatsApp.
•	Inscription anonyme ou profil incomplet visible → éliminé parce que la Contrainte 4 fait de la vérification minimale une condition non négociable de publication.
•	Formulaire d'inscription long en texte libre → éliminé parce que la Contrainte 5 impose une expérience d'onboarding accessible aux prestataires du secteur informel, souvent peu à l'aise avec la saisie écrite.
•	Tableau de bord analytique prestataire (statistiques, taux de conversion) → éliminé parce qu'il suppose une familiarité numérique et une régularité d'usage qui n'existe pas encore à ce stade du produit.
•	Application native iOS → éliminée parce que la Contrainte 1 cible exclusivement Android, seul équipement confirmé dans le persona.
________________________________________
Critère de Validation Final
Le MVP est valide si et seulement si : un prestataire comme Mamadou Diop — plombier indépendant, peu habitué aux formulaires numériques, équipé d'un Android bas de gamme et d'un compte Wave — peut s'inscrire, publier son profil vérifié et recevoir une première demande de client en moins de 10 minutes, sans aide extérieure, et sans avoir aucune raison économique ou pratique de quitter la plateforme pour WhatsApp.

