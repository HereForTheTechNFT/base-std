# 04 — P256, passkeys et verification

P256 est la courbe couramment utilisee par WebAuthn et les passkeys, differente de secp256k1 native aux comptes Ethereum classiques.
Une precompile reduit le cout de verification d une signature P256 par rapport a une implementation Solidity complete.
L appelant doit toutefois valider les tailles, les coordonnees de cle et les scalaires de signature selon le contrat de l interface.
Un retour `false`, un revert et l absence de code systeme sont trois situations que l integration doit distinguer.
La verification de signature ne valide ni l origine WebAuthn, ni le challenge, ni le domaine : ces controles restent applicatifs.
Cette frontiere est essentielle pour construire un wallet Base avec passkey.
Source : [`IP256.sol`](https://github.com/base/base-std/blob/main/src/interfaces/IP256.sol).

[Suite : checklist defensive](05-integration-defensive.md)
