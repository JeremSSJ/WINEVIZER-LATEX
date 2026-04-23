Bonjour Nathalie,

Merci pour ce travail de préparation très structuré — les questions sont pertinentes et couvrent bien les enjeux réels de Winevizer. Je vais répondre point par point, avec le plus de transparence possible.

---

1. ACQUISITION ET ANALYSE DU FUNNEL

Volumes
Depuis le lancement, 585 comptes ont été créés avec un usage minimum (création du restaurant + encodage d'au moins un vin). Sur ces 585, 62 ont souscrit un abonnement payant à un moment donné, soit un taux de conversion d'environ 10,6%. Aujourd'hui, 45 clients sont encore actifs (26 mensuels, 19 annuels).

Taux d'abandon
L'analyse du comportement des non-convertis révèle que l'abandon se produit très tôt dans le parcours : la grande majorité des comptes créés n'encodent presque rien et disparaissent sans jamais percevoir la valeur du produit. Il ne s'agit donc pas d'un problème de conversion à la fin du mois d'essai, mais bien d'un problème d'activation en tout début de funnel.

Canaux d'acquisition (hors inbound)
En dehors du SEO organique (principal canal d'acquisition), deux canaux ont été utilisés pour la prospection active : des campagnes Facebook Ads et du mailing direct aux restaurateurs.

Comportement mensuel vs annuel
Les clients ayant souscrit un abonnement annuel présentent un taux de churn significativement plus faible que les mensuels. Ils sont légèrement moins nombreux (19 annuels vs 26 mensuels) mais représentent un indicateur fort d'engagement et de satisfaction. L'engagement annuel peut être interprété comme un proxy de la confiance accordée à l'outil.

---

2. INTÉGRATION ET PRISE EN MAIN (ONBOARDING)

Délai de valeur
Le temps entre la création du compte et la première perception de valeur dépend largement de la rapidité avec laquelle le restaurateur encode sa carte. L'import PDF (nouveau workflow IA) accélère considérablement ce processus. Pour les non-payants, la reconnaissance IA est désormais entièrement automatique avec un délai maximum de 2 heures. Pour les clients payants, une revue manuelle est effectuée sous 24 à 48 heures afin de garantir la qualité des données.

Conception de l'onboarding
L'onboarding n'a pas encore été formellement structuré autour d'un framework PLG (Product-Led Growth) ou d'un Time-to-Value défini. C'est précisément l'un des axes d'amélioration prioritaires identifiés pour 2026-2027. Le "moment aha" naturel du produit est le moment où le restaurateur voit sa carte des vins en ligne pour la première fois, prête à être scannée par ses clients.

Autonomie utilisateur
Un onboarding guidé entièrement automatisé est en cours de développement. Actuellement, j'intervient manuellement (~1h par client) pour vérifier la qualité des données après import PDF. L'objectif est de supprimer cette étape manuelle grâce à l'automatisation IA.

Frictions remontées
Les principales frictions identifiées sont : la complexité perçue de l'encodage manuel pour les restaurateurs peu technophiles, et le manque d'accompagnement guidé pour les premières étapes.

---

3. PROFILS UTILISATEURS ET COMPORTEMENTS

Profil type des clients les plus fidèles
Les établissements qui tirent le plus de valeur de Winevizer et présentent les meilleurs taux de rétention sont les restaurants étoilés et les bars à vins. Ce sont des établissements où le vin est au cœur de l'expérience client, où la carte est complexe, et où l'accompagnement du client dans le choix du vin est un enjeu réel.

Méthodes d'encodage
Les clients fidèles privilégient l'import CSV & PDF (depuis la mise en place de la reconnaissance IA). L'encodage manuel reste utilisé pour les mises à jour ponctuelles.

Corrélations usage / conversion
Une corrélation positive est observée entre le nombre de vins encodés et la conversion : un client qui a passé du temps à construire sa carte est plus enclin à passer payant, car il a déjà investi dans l'outil. Les données de scan QR par les clients finaux sont collectées mais encore en cours d'analyse systématique.

Données comportementales collectées
Du côté restaurateur : connexions à l'interface admin, modifications de carte, exports. Du côté client final : filtres utilisés, vins consultés, favoris, utilisation du sommelier virtuel. Ces données alimentent les statistiques mises à disposition dans le tableau de bord restaurateur.

---

4. RÉTENTION ET ANALYSE DU CHURN

Analyse de l'attrition
Sur les 20 clients perdus depuis le lancement (62 - 42), l'estimation sur la base des retours recueillis est d'environ 50% de churn involontaire (fermetures de restaurants, marchés à faible adoption digitale) et 50% de churn volontaire (manque d'usage, outil perçu comme non prioritaire). Le churn volontaire représente donc un levier d'amélioration direct via l'onboarding et l'accompagnement.

Relances de paiement
Un système de relances automatiques est en place pour les échecs de paiement, géré via le prestataire de paiement.

Durée de vie moyenne
La plateforme étant jeune, la durée de vie moyenne n'est pas encore statistiquement significative. Le suivi de cette métrique est un objectif de 2026.

---

5. STRATÉGIE PRODUIT ET ROADMAP

Top 3 des fonctionnalités les plus demandées
1. L'ajout de la carte des plats (menu food complet)
2. La connexion à davantage de logiciels de caisse (POS)
3. Plus d'options de personnalisation visuelle de la carte

Sommelier virtuel et ruptures de stock
Cette fonctionnalité est identifiée dans la roadmap. L'objectif à terme est que le sommelier puisse automatiquement proposer des alternatives si un vin est marqué en rupture ou retiré de la carte.

Intégrations POS
Oui, c'est une demande récurrente. Les POS les plus mentionnés par les clients sont : L'Addition, Lightspeed, Odoo, RestoMax et Toast. Des intégrations avec ces systèmes sont envisagées dans la roadmap pour permettre des mises à jour de stock en temps réel.

Paywall PDF en période d'essai
Historiquement, la limitation était liée à une contrainte humaine (revue manuelle). Depuis l'intégration de la reconnaissance IA, l'import PDF va être étendu aux comptes non-payants, avec une limite fixée à 50 vins, ce qui constitue une décision commerciale réfléchie (laisser découvrir la valeur, tout en créant une incitation à passer payant pour les cartes plus larges).

Délai de reconnaissance PDF/photo
Pour les non-payants (traitement automatique IA) : 2 heures maximum. Pour les clients payants (revue manuelle de qualité) : 24 à 48 heures.

Extension vers les menus food
Oui, c'est précisément la fonctionnalité la plus demandée et une orientation stratégique envisagée. L'architecture produit est pensée pour l'accueillir.

---

6. ACCÈS ET RESSOURCES POUR L'AUDIT

Compte de test
Je ne fournis pas de compte administrateur, mais vous pouvez créer un compte gratuit directement sur la plateforme pour évaluer l'expérience utilisateur côté restaurateur : https://app.winevizer.com

Roadmap
Je vais vous transmettre un export de la roadmap (liste de tâches et priorisation) sous format Excel (Winevizer_trello_Export)..

Données analytiques
L'export des données statistiques et analytiques est compliquée mais dites moi si vous voulez des chiffres en particulier.

Séquences d'emails
Je vais vous transmettre les trames d'emails d'onboarding et de nurturing utilisées, avec leurs déclencheurs (funnel.pdf).

Exemple de travail précédent
Je vous joins un travail de l'année passée.

---

N'hésitez pas à revenir vers moi si certaines réponses méritent d'être approfondies. Je reste disponible pour un éventuel appel de suivi si cela est utile à votre analyse.

Bonne continuation dans votre travail,