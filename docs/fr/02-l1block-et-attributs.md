# 02 — L1Block et attributs L1

La precompile L1Block expose au contexte L2 des attributs derives de la couche 1 et du traitement OP Stack.
Ces valeurs servent notamment a tarifer les donnees et a relier l execution L2 a son origine L1.
Elles ne doivent pas etre interpretees comme un oracle metier generaliste.
Selon l attribut, la valeur peut evoluer avec les mises a niveau du protocole et le format de cout des donnees.
Une application doit eviter de figer des hypotheses implicites sur les coefficients ou l epoque de tarification.
La bonne pratique est d utiliser l interface officielle et de documenter l invariant reellement necessaire.
Source : [`IL1Block.sol`](https://github.com/base/base-std/blob/main/src/interfaces/IL1Block.sol).

[Suite : Superchain](03-superchain-et-identite.md)
