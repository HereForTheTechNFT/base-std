# 9 — Invariants NFT avec passkeys

Une passkey améliore l’expérience de signature mais ne remplace pas les contrôles économiques du contrat NFT.
Le mint conserve plafonds, fenêtres, allowlist, paiement et protection contre la réentrance indépendamment du signataire.
Le destinataire engagé doit être celui qui reçoit réellement le token ou l’autorisation de transfert.
Une signature ne doit pas pouvoir changer de collection, de tokenId ou de montant après validation.
Les opérations par lot nécessitent un hash déterministe de l’ordre et du contenu des éléments.
La récupération de compte doit avoir une temporisation et une portée qui n’annulent pas les garanties anti-rejeu.
Ce parcours est documentaire : aucune installation, compilation, transaction ou exécution de tests.
Les invariants doivent être confrontés aux tests et interfaces du dépôt avant déploiement.
