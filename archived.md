Plusieurs options d'authentification moins friables se présentent~: un \textit{magic link} par
email (un seul champ, pas de mot de passe initial), un OTP à six chiffres (également combinable
avec la création automatique de compte à partir d'un upload PDF, voir R3) ou un \textit{social
login} Google/Apple (moindre effort utilisateur mais dépendance aux tiers). En parallèle,
retirer le champ \og{}confirmation de mot de passe\fg{} au profit d'un \textit{toggle}
afficher/masquer, exposer les règles avant la saisie, et soit supprimer la confirmation email
bloquante (si non requise légalement, à vérifier) soit auto-authentifier l'utilisateur au clic
sur le lien. Le KPI prioritaire est le taux de passage \og{}compte créé $\rightarrow$
établissement créé\fg{}, aujourd'hui première étape de perte (20\,\%), avec une cible inférieure
à 5\,\%. Effort~: deux à cinq jours-homme.

\subsection{R3 — Faire de l'import PDF la porte d'entrée principale}

L'import PDF est le seul point d'entrée naturel pour un restaurateur disposant déjà d'une
carte papier, pourtant il est aujourd'hui à la fois le plus caché (widget secondaire, onglet
peu visible) et le seul verrouillé derrière le paywall. Première option~: l'ouvrir aux comptes
gratuits avec un quota de 50 vins (plan déjà évoqué par le fondateur), l'\textit{upsell}
intervenant naturellement au dépassement. Option plus structurante~: placer l'upload PDF en
point d'entrée unique depuis la landing page, avec création automatique de compte et accès par
OTP, le chemin manuel/CSV devenant secondaire via un bouton \og{}je n'ai pas de carte à
importer\fg{}. Cette inversion élimine à elle seule le principal goulot d'onboarding. L'option
de statu quo avec tutoriels vidéo enrichis compenserait un problème d'architecture par du
contenu et est à écarter. Risque résiduel~: l'email contenant le lien d'accès peut se perdre
(spam, suppression)~; l'OTP rechargeable à la demande (R2) le neutralise. KPI~: taux
d'atteinte du moment \og{}aha\fg{} (carte en ligne + QR code généré) à J+1, cible $>$40\,\%.

\subsection{R4 — Redesign de l'onboarding autour du Time-to-Value}

Le parcours doit être restructuré pour livrer une valeur intermédiaire tangible à chaque étape,
plutôt que de la repousser à la fin. Quatre axes non exclusifs~: un profilage progressif (à la
création, n'exiger que nom et pays, le reste étant demandé au moment utile)~; un aperçu
immédiat (dès trois à cinq vins importés, générer un QR code de prévisualisation et notifier
\og{}votre carte est en ligne, voici à quoi elle ressemble sur smartphone\fg{})~; un guide
d'onboarding relançable avec centre d'aide et tutoriels vidéo intégrés (le \og{}Ne plus voir
l'aide\fg{} actuel n'est pas réversible)~; et une distinction claire entre chatbot FAQ et
support humain, pour aligner l'attente de l'utilisateur sur le SLA soutenable par l'équipe
actuelle. Effort cumulé~: quatre à huit semaines-développeur, priorisables par sprint. KPI~:
temps médian entre création du compte et génération du premier QR code, cible inférieure à
30 minutes sur le chemin PDF.

\subsection{R5 — Gestion automatisée des échecs de paiement}

Un système de relance existe déjà via le prestataire de paiement~; il s'agit de le formaliser.
Séquence \textit{dunning} en trois étapes~: J+0 retry automatique, J+3 email de relance, J+7
email avec mise à jour du moyen de paiement en un clic~; complétée par un flux \textit{win-back}
à J+15 pour les annulations volontaires. Si le prestataire actuel ne couvre pas ce scénario
nativement, un outil tiers (Stripe Smart Retries, Chargebee) peut être ajouté à moindre coût.
KPI~: taux de récupération des paiements échoués (benchmark SaaS~: 30 à 70\,\% avec un
\textit{dunning} mature).

\subsection{R6 — Système d'alerte précoce de churn}

Le churn volontaire représente environ la moitié des sorties~; c'est le seul levier directement
actionnable. Définir trois à cinq indicateurs comportementaux de pré-churn sur la base des
abonnés payants (baisse des scans QR hebdomadaires, absence de connexion au back-office
depuis 30 jours, baisse du taux de validation des suggestions, carte non mise à jour depuis 60
jours) et déclencher automatiquement soit un email de \textit{check-in}, soit, pour les
abonnés annuels à forte valeur, un appel de \textit{customer success} du fondateur ou du
futur commercial. Cette métrique est à distinguer strictement des indicateurs d'activation et
de conversion de R1 à R4, qui portent sur la base non payante~: les confondre brouillerait le
pilotage. Effort~: requêtes SQL sur la base existante et intégration à l'outil d'emailing
déjà en place. KPI~: churn volontaire à 12 mois, cible $-30\,\%$ en deux ans.

\subsection{R7 — Programme de fidélisation et parrainage}

Trois options complémentaires~: parrainage client-à-client (un mois offert pour tout abonné
apportant un confrère)~; gamification des paliers d'encodage pendant l'essai (flyers de table
offerts au 50\textsuperscript{e} vin encodé, idée déjà identifiée par le fondateur dans le
Cas~5)~; programme de fidélité pour abonnés annuels (remise sur la deuxième année, accès
anticipé aux nouvelles fonctionnalités). La littérature SaaS suggère qu'un programme de
parrainage bien conçu peut générer 10 à 20\,\% des nouvelles acquisitions d'un outil B2B, à
coût très inférieur à l'outbound. KPI~: part des nouveaux abonnements issus du parrainage et
taux de renouvellement annuel.

\subsection{R8 — Différenciation défensive face aux substituts}

Face à Somm'it, positionner Winevizer sur le segment non adressé par le concurrent, à savoir le petit
restaurant et le bar à vins indépendants (moins de 100 références), où le sommelier virtuel
apporte plus de valeur qu'un back-office de gestion de stock avancé. Face à l'IA générative
grand public, la défense repose sur trois différenciateurs à exposer explicitement dans la
communication (R1)~: la restriction au stock réel de l'établissement (ChatGPT peut suggérer
un Romanée-Conti absent de la cave), la boucle de données comportementales accumulée sur
trois ans, et l'intégration POS/stock hors de portée d'un assistant généraliste. Option
complémentaire à arbitrer selon l'effort~: protection juridique (marque déposée, éventuel
brevet sur la méthode de recommandation contextualisée au stock), qui répond à la crainte
principale exprimée par le fondateur quant à la duplication par IA.

\subsection{R9 — Boucle de fraude sur l'essai gratuit}

Il est actuellement possible de supprimer un compte et de le recréer avec la même adresse
email, sans traçabilité de l'essai déjà consommé. Deux options~: marquer l'adresse email (et
l'IP, et le nom d'établissement) comme \og{}déjà essayée\fg{} en base, indépendamment de la
suppression du compte (effort minimal, efficace contre l'abus naïf)~; ou exiger une empreinte
de paiement à la création du compte, non débitée pendant l'essai, qui réduit drastiquement la
fraude mais introduit une friction au sign-up à mettre en balance avec R2. KPI~: nombre de
comptes essai par adresse email (attendu~: 1).

\subsection*{Conclusion}

R1 à R4 et R9, tous à effort faible et impact majeur, sont activables par l'équipe actuelle
dans les semaines qui suivent le rendu de ce rapport et devraient, à elles seules, déplacer
significativement l'indicateur d'activation. R4, R5 et R8 s'inscrivent dans le chantier produit
du semestre post-passage en société, parallèlement au recrutement commercial. R6 et R7 ne
prennent leur sens qu'une fois la base d'abonnés consolidée~: tenter de réduire le churn avant
d'avoir fiabilisé l'activation reviendrait à optimiser un entonnoir percé par le haut. Cet
ordonnancement respecte la logique causale du problème diagnostiqué~: sans abonnés, pas de
rétention~; sans activation, pas d'abonnés~; sans compréhension de la valeur, pas d'activation.