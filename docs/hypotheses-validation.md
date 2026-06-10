Hypothèses de Validation — Groupe Business
HMW Définitif
Comment pourrions-nous faciliter la mise en relation entre prestataires de services et clients à Dakar, en construisant un système de confiance adapté aux usages mobiles locaux, afin que la recherche, la sélection et la collaboration soient plus simples, rapides et fiables — y compris pour les prestataires peu connectés ?
________________________________________
Hypothèses CRITIQUES
(Si fausse → le MVP ne fonctionne pas)
Hypothèse C1 — Désintermédiation
Affirmation : Nous croyons que les prestataires et les clients resteront sur la plateforme après le premier contact si elle leur offre des avantages exclusifs introuvables sur WhatsApp : historique de transactions certifié, évaluations visibles, et protection en cas de litige.
Indicateur : Nous le saurons si, lors de 5 entretiens avec des prestataires réels à Dakar, au moins 3 déclarent qu'ils seraient prêts à payer une commission ou à rester sur la plateforme en échange de ces garanties — et identifient spontanément au moins un avantage qu'ils ne peuvent pas obtenir via WhatsApp.
Méthode : Entretien semi-directif terrain avec scénario simulé — montrer une maquette du profil avec historique + évaluation et demander : "Est-ce que ça change quelque chose pour vous par rapport à WhatsApp ?"
Qui valide : Elhadji Omar Diallo (Développeur UI) prépare la maquette ; Merveille Atipot (PM) conduit les entretiens avec des plombiers, électriciens ou maçons dans les quartiers de Médina, Parcelles Assainies ou Grand-Yoff.
Délai S3 : Semaine 1 — priorité absolue avant tout développement.
________________________________________
Hypothèse C2 — Accessibilité numérique
Affirmation : Nous croyons qu'un prestataire informel peu habitué aux formulaires numériques, comme Mamadou Diop, est capable de créer un profil complet et utilisable sur notre plateforme en moins de 10 minutes, sans aide extérieure, depuis un smartphone Android d'entrée de gamme.
Indicateur : Nous le saurons si, lors d'un test d'utilisabilité sur prototype papier ou Figma avec 3 prestataires réels, au moins 2 complètent le flux d'inscription sans blocage critique et sans poser plus de 2 questions à l'observateur.
Méthode : Test utilisateur en observation silencieuse — le testeur ne doit pas intervenir ; noter chaque hésitation, abandon ou erreur de navigation.
Qui valide : Rokhaya (Responsable Impact) recrute les testeurs dans le réseau terrain ; Fatima (Prompt Engineer) documente les points de friction observés.
Délai S3 : Semaine 1 — en parallèle de C1, sur prototype basse fidélité.
________________________________________
Hypothèse C3 — Confiance et vérification
Affirmation : Nous croyons que les clients refuseront de contacter un prestataire sans évaluation vérifiée ou sans preuve d'identité visible sur son profil, rendant un mécanisme de confiance minimal indispensable dès le lancement.
Indicateur : Nous le saurons si, lors de 5 entretiens avec des clients potentiels (particuliers ou petites entreprises à Dakar), au moins 4 déclarent qu'ils n'utiliseraient pas la plateforme si les profils ne sont pas vérifiés ou évalués par d'autres utilisateurs.
Méthode : Entretien avec mise en situation — présenter deux profils fictifs : l'un sans photo ni évaluation, l'autre avec photo + 3 avis clients. Observer et enregistrer la réaction spontanée.
Qui valide : Merveille Atipot conduit les entretiens ; Rokhaya analyse les réponses sous l'angle impact social et inclusion.
Délai S3 : Semaine 2 — après C1 et C2, pour confirmer le niveau minimal de confiance requis.
________________________________________
Hypothèses IMPORTANTES
(Si fausse → expérience dégradée mais MVP utilisable)
Hypothèse I1 — Adoption de Wave comme paiement
Affirmation : Nous croyons que Mamadou Diop et ses clients sont à l'aise pour effectuer ou recevoir un paiement de service via Wave directement depuis la plateforme, sans friction supplémentaire liée à l'intégration.
Indicateur : Nous le saurons si, lors des entretiens terrain, au moins 4 prestataires sur 5 confirment utiliser Wave régulièrement pour recevoir des paiements de clients, et qu'aucun ne mentionne de blocage technique récurrent.
Méthode : Question directe en entretien + observation : "Comment vous êtes-vous fait payer la dernière fois ?" Vérifier si Wave est déjà dans les habitudes sans suggestion de l'enquêteur.
Qui valide : Fatima en entretien ; Elhadji Omar documente les cas d'usage réels pour la conception du flux paiement.
Délai S3 : Semaine 2 — en parallèle de C3.
________________________________________
Hypothèse I2 — Couverture réseau et data suffisante
Affirmation : Nous croyons que les prestataires cibles dans les quartiers populaires de Dakar (Médina, Pikine, Guédiawaye) disposent d'une connexion 3G suffisante pour charger et utiliser la plateforme sans interruption majeure dans leur quotidien de travail.
Indicateur : Nous le saurons si, lors des tests terrain, l'application prototype se charge en moins de 5 secondes sur réseau 3G dans au moins 3 quartiers cibles différents, et que les prestataires ne mentionnent pas spontanément le réseau comme frein.
Méthode : Test technique terrain — charger le prototype depuis un téléphone Android avec SIM locale en 3G dans les quartiers cibles ; chronométrer et noter les coupures.
Qui valide : Elhadji Omar Diallo effectue les tests techniques terrain avec son propre téléphone ou un téléphone emprunté.
Délai S3 : Semaine 2.
________________________________________
Hypothèses SECONDAIRES
(À valider après le MVP)
Hypothèse S1 — Monétisation acceptable par les prestataires
Affirmation : Nous croyons que les prestataires accepteront de payer une commission sur les missions trouvées via la plateforme une fois qu'ils auront constaté une valeur concrète (au moins une mission conclue).
Indicateur : Nous le saurons si, après 4 semaines d'usage réel du MVP, au moins 60% des prestataires actifs déclarent être prêts à payer entre 3% et 8% de commission par mission réussie.
Méthode : Enquête courte post-usage (5 questions via formulaire WhatsApp ou appel direct).
Qui valide : Merveille Atipot (PM) analyse les résultats ; Rokhaya évalue l'impact sur les revenus des prestataires.
Délai : Post-lancement MVP — semaine 4 ou 5.
________________________________________
Hypothèse S2 — Bouche-à-oreille comme canal d'acquisition
Affirmation : Nous croyons que les premiers prestataires satisfaits recommanderont spontanément la plateforme à leurs pairs, générant une croissance organique sans budget marketing.
Indicateur : Nous le saurons si, après le premier mois de MVP, au moins 30% des nouvelles inscriptions prestataires mentionnent avoir entendu parler de la plateforme par un autre prestataire.
Méthode : Question systématique à l'inscription : "Comment avez-vous connu notre plateforme ?" + analyse des sources d'acquisition.
Qui valide : Fatima (Prompt Engineer) met en place le tracking de la question ; Merveille consolide les données.
Délai : Post-lancement MVP — semaine 4 à 6.
________________________________________
Priorité de Validation S3
La première chose à tester en S3 : organiser dès la semaine 1 des entretiens terrain avec 5 prestataires réels dans les quartiers de Médina ou Parcelles Assainies pour valider simultanément C1 (risque de désintermédiation) et C2 (accessibilité numérique) — car si l'une de ces deux hypothèses est fausse, le MVP doit être repensé avant toute ligne de code.

