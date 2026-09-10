# 03 — Superchain et identite de chaine

Les interfaces Superchain donnent acces a des informations partagees ou coordonnees entre chaines de l ecosysteme OP.
L identifiant de chaine reste une donnee de securite : une signature ou autorisation ne doit pas etre reutilisee sur une autre chaine par accident.
Les adresses systeme et fonctionnalites disponibles peuvent differer selon le deploiement ou l etape de mise a niveau.
Avant appel, une application doit connaitre le reseau cible et prevoir explicitement l indisponibilite de la precompile.
Pour les signatures, inclure le domaine et le chain ID evite qu une preuve d intention soit acceptee dans un autre contexte.
La composabilite interchaine exige davantage de domaine, pas moins.
Source : [`interfaces`](https://github.com/base/base-std/tree/main/src/interfaces).

[Suite : P256](04-p256-et-passkeys.md)
