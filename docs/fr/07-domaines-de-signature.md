# 7 — Domaines de signature et anti-rejeu

Une signature P256 prouve la possession d’une clé, pas l’intention complète de l’utilisateur.
Le message signé doit engager chaîne, contrat, fonction, nonce, échéance et paramètres NFT pertinents.
Sans séparation de domaine, une preuve valide peut être rejouée dans un autre contrat ou environnement.
Le nonce doit être consommé atomiquement avec l’action et ne jamais dépendre du seul horodatage.
Pour un mint, engager collection, destinataire, quantité, prix et plafond évite la substitution de paramètres.
Une rotation de clé doit révoquer clairement les anciennes autorisations encore valides.
Le format de hash doit être canonique et identique entre wallet, backend et contrat.

Suite : [résultats P256](08-resultats-p256.md).
