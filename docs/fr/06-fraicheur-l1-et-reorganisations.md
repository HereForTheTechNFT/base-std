# 6 — Fraîcheur L1 et réorganisations

L1Block expose à Solidity des attributs dérivés de la chaîne L1, mais leur présence ne signifie pas finalité immédiate.
Une application doit distinguer numéro, horodatage, hash et séquence utilisés par sa règle métier.
Un prix, une racine ou une autorisation liée au contexte L1 doit porter une limite de fraîcheur explicite.
Les états unsafe, safe et finalized ne sont pas interchangeables pour une opération irréversible.
Une réorganisation peut invalider une observation récente sans rendre défectueuse la précompile elle-même.
Pour un mint ou une révélation NFT, le contrat doit définir le niveau de confirmation attendu avant consommation définitive.
Les événements doivent conserver le contexte observé afin de rendre la décision audit-able après coup.

Suite : [domaines de signature](07-domaines-de-signature.md).
