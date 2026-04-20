# Projet en Python : Utilitaire - regroupement conditionnel de rows temporelles au sein d’un groupby de columns
- création des dates de debut et de fin de périodes temporelles par identifiant de la table
- remplissage des valeurs nulles par forward propagation des informations non nulles
- fonction conditionnelle de concaténation des informations temporelles contenues en ligne par comparaison avec la ligne précédente au sein d’un group by
	- si row(r)=row(r-1) => concaténation
	- si row(r)!=row(r-1) => séparation en deux rows
