# 05 — Checklist d integration defensive

1. Verifier le chain ID et la disponibilite attendue de la precompile.
2. Encoder les entrees avec l interface officielle et controler leur domaine avant l appel.
3. Distinguer succes d appel, validite du resultat, revert et retour mal forme.
4. Ne jamais supposer qu un mock reproduit le cout en gas ou toutes les erreurs du client.
5. Versionner l hypothese de protocole avec la fonctionnalite applicative qui en depend.
6. Pour P256, verifier aussi challenge, origine, domaine et politique de compte hors de la precompile.
Ce parcours est documentaire, pas un audit. Aucune installation, compilation ou execution de tests n a ete effectuee.
Source de verification future : [`test`](https://github.com/base/base-std/tree/main/test).

[Retour au sommaire](README.md)
