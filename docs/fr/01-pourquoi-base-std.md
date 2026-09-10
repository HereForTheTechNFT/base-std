# 01 — Pourquoi base-std

`base-std` rassemble des interfaces, bibliotheques et mocks pour les precompiles exposes par Base.
Une precompile ressemble a un contrat a adresse connue, mais son comportement est implemente par le client plutot que par du bytecode ordinaire.
La bibliotheque fournit une surface Solidity stable et rend les appels plus lisibles dans les applications.
Les mocks permettent de raisonner sur ces interfaces hors du reseau, sans pretendre reproduire toutes les proprietes du client.
Une integration doit verifier chaine, adresse, format des entrees, forme du retour et comportement en cas d echec.
Le parcours distingue donc convention d interface et garantie du protocole sous-jacent.
Source : [`src`](https://github.com/base/base-std/tree/main/src).

[Suite : L1Block](02-l1block-et-attributs.md)
