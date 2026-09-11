# 8 — Résultats P256 et politique d’échec

La vérification P256 renvoie une décision cryptographique qui doit rester distincte d’un échec d’appel à la précompile.
Un retour mal formé, trop court ou indisponible ne doit jamais être assimilé à une signature valide.
Le contrat appelant doit choisir explicitement entre revert, refus booléen et chemin de repli.
Un repli logiciel élargit la surface de code et doit préserver exactement les mêmes règles d’encodage.
Les coordonnées de clé et composantes de signature doivent respecter les bornes et formats attendus.
Une politique multi-signature ou de récupération ne doit pas contourner le nonce du chemin passkey.
La télémétrie doit distinguer signature invalide, entrée invalide et infrastructure indisponible.

Suite : [invariants NFT](09-invariants-nft-passkeys.md).
