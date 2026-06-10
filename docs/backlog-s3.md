Backlog S3 — Groupe Business
HMW Définitif
Comment pourrions-nous faciliter la mise en relation entre prestataires de services et clients à Dakar, en construisant un système de confiance adapté aux usages mobiles locaux, afin que la recherche, la sélection et la collaboration soient plus simples, rapides et fiables — y compris pour les prestataires peu connectés ?
________________________________________
User Stories MUST
(À construire obligatoirement en S3)
US-01 — Inscription et profil prestataire vérifié
Story : En tant que Mamadou Diop, plombier indépendant, je veux créer mon profil professionnel en moins de 5 minutes avec des listes déroulantes, une photo et mon numéro Wave, afin d'exister numériquement et d'apparaître dans les résultats de recherche des clients.
Priorité : MUST
Outil : Bolt.new (formulaire d'inscription) + Dify (validation et modération du profil)
Effort : Moyen — formulaire simple dans Bolt.new mais la logique de validation Wave + activation par modérateur nécessite une configuration Dify précise
Adresse : Pain Reliever — Faux profils et arnaques → vérification obligatoire numéro Wave + photo + validation modérateur humain ; Contrainte 4 et Contrainte 5
Critère d'acceptation : Un prestataire peut créer un profil complet (catégorie, quartier, photo, numéro Wave) en moins de 5 minutes depuis un Android 3G ; le profil n'apparaît dans aucun résultat de recherche tant que le modérateur ne l'a pas activé manuellement ; testé avec 2 prestataires réels en observation silencieuse.
________________________________________
US-02 — Publication d'une demande de service par un client
Story : En tant que client particulier à Dakar, je veux publier une demande de service en choisissant une catégorie, un quartier et en décrivant mon besoin en quelques mots, afin de trouver rapidement un prestataire disponible près de chez moi.
Priorité : MUST
Outil : Bolt.new (formulaire de demande client) + Dify (traitement et routage de la demande vers les prestataires correspondants)
Effort : Moyen — le formulaire est simple mais le routage automatique vers les bons prestataires (par catégorie + quartier) nécessite une logique Dify à configurer soigneusement
Adresse : Gain Creator — Flux critique prototypé en priorité → parcours inscription → demande client → mise en relation → premier contact ; Contrainte 1
Critère d'acceptation : Un client peut publier une demande en moins de 3 minutes depuis un Android 3G ; la demande est automatiquement visible pour les prestataires de la bonne catégorie dans le bon quartier ; le poids de la page de formulaire ne dépasse pas 200 Ko.
________________________________________
US-03 — Mise en relation et premier contact sécurisé
Story : En tant que Mamadou Diop, je veux recevoir une notification dès qu'une demande correspond à mon profil et pouvoir contacter le client directement depuis GalleExpress, afin de ne manquer aucune opportunité de mission sans devoir chercher activement.
Priorité : MUST
Outil : Dify (déclenchement de la notification) + SMS API — Orange SMS ou Twilio (alerte SMS si pas de connexion data) + Bolt.new (interface de mise en relation)
Effort : Élevé — l'intégration SMS API est la partie la plus technique pour une équipe no-code débutante ; prévoir un plan de secours par notification WhatsApp Business si l'API SMS bloque
Adresse : Gain Creator — Réduction du temps de prospection → alertes géolocalisées supprimant la recherche active ; Pain Reliever — Désintermédiation → premier contact tracé dans GalleExpress, pas hors plateforme ; Contrainte 3
Critère d'acceptation : Dès qu'une demande est publiée, le prestataire correspondant reçoit une alerte SMS ou notification dans les 2 minutes ; le premier échange entre client et prestataire est enregistré dans l'historique GalleExpress ; le contact ne contient pas le numéro personnel du prestataire avant validation mutuelle.
________________________________________
US-04 — Modération manuelle des profils par le responsable désigné
Story : En tant que modérateur de GalleExpress (Rokhaya, Responsable Impact), je veux consulter la liste des profils prestataires en attente de validation et les activer ou refuser en un clic, afin de garantir que chaque prestataire visible dans les résultats est vérifié et fiable.
Priorité : MUST
Outil : Dify (tableau de modération) + Bolt.new (interface admin légère)
Effort : Faible — une vue liste avec boutons Activer / Refuser suffit pour le MVP ; pas besoin d'une interface complexe
Adresse : Pain Reliever — Faux profils et arnaques → validation modérateur humain avant toute visibilité ; Gain Creator — Confiance active dès le lancement ; Contrainte 4
Critère d'acceptation : Le modérateur peut voir tous les profils en attente, consulter la photo et le numéro Wave, et activer ou refuser un profil en moins de 30 secondes ; un profil refusé ne réapparaît jamais dans les résultats sans nouvelle soumission.
________________________________________
User Stories SHOULD
(À construire si le temps le permet)
US-05 — Évaluation post-mission par le client
Story : En tant que client ayant reçu un service, je veux laisser une note et un commentaire court sur le prestataire depuis GalleExpress, afin d'aider les futurs clients à choisir en confiance et de récompenser les bons prestataires.
Priorité : SHOULD
Outil : Bolt.new (formulaire d'évaluation 1 à 5 étoiles + commentaire court) + Dify (mise à jour automatique de la note moyenne sur le profil)
Effort : Faible — formulaire simple, logique de calcul de moyenne configurable dans Dify
Adresse : Gain Creator — Visibilité professionnelle crédible → profil évalué visible ; Pain Reliever — Désintermédiation → rester sur GalleExpress apporte un historique d'évaluations impossible à reproduire sur WhatsApp ; Contrainte 3
Critère d'acceptation : Après confirmation d'une mission, le client reçoit un lien d'évaluation ; la note s'affiche sur le profil public du prestataire dans les 5 minutes suivant la soumission.
________________________________________
US-06 — Historique des missions pour le prestataire
Story : En tant que Mamadou Diop, je veux consulter la liste de toutes mes missions passées sur GalleExpress avec les évaluations reçues, afin de prouver mon expérience à de nouveaux clients sans dépendre du bouche-à-oreille.
Priorité : SHOULD
Outil : Bolt.new (page historique prestataire) + Dify (consolidation des données de missions)
Effort : Moyen — nécessite une base de données structurée dès US-01 et US-03 pour être alimentée automatiquement
Adresse : Gain Creator — Visibilité professionnelle crédible ; Pain Reliever — Désintermédiation → valeur exclusive impossible à obtenir hors GalleExpress ; Contrainte 3
Critère d'acceptation : Le prestataire voit sur son profil le nombre de missions complétées, la note moyenne et les 3 derniers commentaires clients ; ces données sont visibles aussi par les clients consultant le profil.
________________________________________
User Stories COULD
(Roadmap post-MVP)
US-07 — Création de profil par message vocal
Story : En tant que Mamadou Diop, peu à l'aise avec la saisie écrite, je veux enregistrer un message vocal décrivant mes services afin que mon profil soit créé automatiquement sans remplir de formulaire.
Priorité : COULD
Outil : Dify (transcription audio-to-text) + Bolt.new (intégration du champ vocal dans le formulaire)
Effort : Élevé — dépend de la qualité de la transcription en wolof / français mixé, non fiable sans test terrain approfondi ; à valider après MVP
Adresse : Pain Reliever — Fracture numérique fonctionnelle ; Contrainte 5
Critère d'acceptation : Un prestataire enregistre un message vocal de 30 secondes maximum ; le texte transcrit est affiché pour correction avant validation ; le profil est créé sans aucune saisie clavier obligatoire.
________________________________________
US-08 — Système de certification communautaire (tontine numérique)
Story : En tant que client vérifié, je veux recommander un prestataire de confiance afin qu'il obtienne un badge "Certifié GalleExpress" visible sur son profil lorsque 3 clients vérifiés l'ont recommandé.
Priorité : COULD
Outil : Dify (compteur de recommandations + déclenchement du badge) + Bolt.new (affichage du badge sur le profil)
Effort : Moyen — logique de comptage simple dans Dify mais nécessite une base de clients vérifiés suffisante pour être utile ; prématuré avant d'avoir 20+ utilisateurs actifs
Adresse : Pain Reliever — Faux profils et arnaques → validation communautaire en complément de la modération humaine ; Gain Creator — Confiance active
Critère d'acceptation : Dès que 3 clients vérifiés recommandent un prestataire, le badge apparaît automatiquement sur son profil public ; le compteur est visible et non falsifiable.
________________________________________
Sprint S3
Semaine 1 : Construire US-01 (profil prestataire vérifié) + US-04 (interface de modération) — ces deux stories forment le socle sans lequel rien d'autre ne fonctionne ; tester US-01 avec 2 prestataires réels en fin de semaine 1 pour détecter les blocages d'inscription avant de continuer.
Semaine 2 : Construire US-02 (publication demande client) + US-03 (mise en relation + alerte SMS) — intégrer le SMS API en début de semaine 2 pour avoir le temps de déboguer ; si l'API SMS bloque, basculer sur notification WhatsApp Business comme plan de secours documenté.
Démo S6 : Démontrer en live le flux complet US-01 → US-02 → US-03 → US-04 : un prestataire crée son profil → le modérateur l'active → un client publie une demande → le prestataire reçoit une alerte et prend contact depuis GalleExpress — tout le flux en moins de 10 minutes, depuis un smartphone Android réel.

