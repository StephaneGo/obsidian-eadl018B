
Date: 18/11/2026
Tags: [Design pattern]


# Questions

> [!info]- Les 2 BDD doivent-elles obligatoirement être du même type ?
> Non, les 2 BDD peuvent être différentes : BDD relationnelle pour l'écriture, et BDD NoSQL (basé sur les documents) pour la lecture (+ efficace).

# Notes
### Principe 
>Séparer les opérations de lecture (*queries*) des opérations d'écriture (*commands*). Pour cela, on utilise 2 BDD, une pour chaque type d'opération. **Les 2 doivent rester synchronisées.**


Ca permet de gagner en performance (latence / débit de donnée).
![[Pasted image 20261118154559.png]]


# Références
https://medium.com/@minekayaa/cqrs-design-pattern-series-423aeff781e4