---
title: "Comment créer des nomenclatures de production"
description: "Une nomenclature de production contient les données de base qui décrivent les composantes et les sous-ensembles utilisés lors de la production d'un article parent. Après la création d'un bon de production pour cet article parent, sa nomenclature de production régira le calcul des besoins matière tels que représentés dans la fenêtre **Composantes bon de production**."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/05/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 122bc1fa0b259e4d80ad134b94abcdc4d2d96640
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-production-boms"></a>Comment créer des nomenclatures de production
Une nomenclature de production contient les données de base qui décrivent les composantes et les sous-assemblages utilisés lors de la production d'un article parent. Après la création d'un ordre de fabrication pour cet article parent, sa nomenclature de production gouvernera le calcul de besoins matériels tels que représentés dans la fenêtre **Composants ordre prod.**.

[!INCLUDE[d365fin](includes/d365fin_md.md)] prend également en charge les nomenclatures d'assemblage. Vous utilisez des ordres d'assemblage pour fabriquer des produits finis à partir de composants dans le cadre d'un processus simple qui peut être exécuté par une ou plusieurs ressources de base, qui ne sont pas des postes ou centres de charge, ou sans ressource. Par exemple, un processus d'assemblage peut consister à prélever deux bouteilles de vin et un sachet de café puis à les emballer comme article de cadeau. Pour plus d'informations, voir la section « Nomenclatures d'assemblage ou nomenclatures de production » dans [Procédure : utiliser les nomenclatures](inventory-how-work-BOMs.md).  

Pour pouvoir configurer un itinéraire, les éléments suivants doivent être en place :  

- Des fiches article sont créées pour les articles parents qui participent à la production. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux articles](inventory-how-register-new-items.md).
- Les ressources de production sont configurées. Pour plus d'informations, voir [Procédure : configurer des ateliers et des unités de production](production-how-to-set-up-work-and-machine-centers.md).

## <a name="to-create-a-production-bom"></a>Pour créer une nomenclature de production  
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Nomenclature de production**, puis sélectionnez le lien associé.  
2. Sélectionnez l'action **Nouveau**.  
3. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Pour modifier la nomenclature, définissez le champ **Statut** sur **Création en cours** ou sur **Modification en cours**. Pour l'activer, définissez le champ **Statut** sur **Validée**.  

    Renseignez les lignes nomenclature de production.
5. Dans le champ **Type**, indiquez si l'article sur la ligne nomenclature est un article ordinaire ou s'il s'agit d'une nomenclature de production. Dans le dernier cas, l'article doit déjà exister en tant que nomenclature de production certifiée.  
6.  Dans le champ **N°**, consultez et sélectionnez l'article ou la nomenclature de production concernée \(ou entrez l'un ou l'autre\).  
7.  Dans le champ **Quantité par**, spécifiez le nombre d'unités de l'article intégrant l'article parent, par exemple, les 4 roues d'une voiture.  
8.  Dans le champ **% rebut**, vous pouvez indiquer le taux fixe de perte de composants lors de la production. Une fois qu'ils sont prêts à être consommés dans un ordre de fabrication lancé, ce taux est ajouté à la quantité prévue dans le champ **Quantité consommée** dans une feuille production. Pour plus d'informations, reportez vous à [Comment enregistrer la consommation et la production](production-how-to-register-consumption-and-output.md).  

    > [!NOTE]  
    >  Ce pourcentage de rebut correspond aux composantes mises au rebut au cours de la production, durant le prélèvement de l'inventaire. Sur les lignes itinéraire, il représente la production mise au rebut avant la constitution de l'inventaire.  

9.  Dans le champ **Code lien gamme**, vous pouvez entrer un code permettant de lier le composant à une opération spécifique. Pour plus d'informations, voir la section « Pour créer des liens itinéraire » dans [Procédure : créer des itinéraires](production-how-to-create-routings.md).
10. Pour copier des lignes à partir d'une nomenclature de production existante, choisissez l'action **Copier nomenclature** pour sélectionner des lignes existantes.  
11.  Certifiez la nomenclature de production.  
12.  Vous pouvez désormais joindre la nouvelle nomenclature de production à la fiche de l'article parent en question. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux articles](inventory-how-register-new-items.md).  

> [!NOTE]  
>  Pour recalculer le coût standard de l'article figurant sur la fiche article, choisissez l'action **Production**, puis l'action **Calculer coût standard**.  

## <a name="to-create-a-new-versions-of-a-production-bom"></a>Pour créer une nouvelle version d'une nomenclature de production
Les nouvelles versions des nomenclatures de production sont utilisées lorsque, par exemple, un article est remplacé par un autre article, ou lorsqu'un client demande une version spéciale d'un produit. Le principe de la version permet de gérer différentes versions d'une nomenclature de production. La structure des versions de nomenclature de production correspond à celle des nomenclatures de production. La principale différence réside dans la validité des versions. La validité est définie par la date début.  

La date début indique le début de la période de validité de la version. La date début peut également être considérée comme un filtre pour les calculs et les évaluations. La version de la nomenclature est valide jusqu'à l'entrée en vigueur de la version suivante, qui est indiquée par sa date début.  

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Nomenclature de production**, puis sélectionnez le lien associé.  
2.  Sélectionnez la nomenclature de production à copier, puis choisissez l'action **Versions**.  
3.  Sous l'onglet de **Accueil**, dans le groupe **Nouveau**, choisissez **Nouveau**.  
4. Renseignez les champs selon vos besoins.
5. Dans le champ **Code version**, saisissez le numéro d'identification unique de la version. Ce champ admet n'importe quelle combinaison de chiffres et de lettres.  

    Le statut **Nouveau** est automatiquement affecté à la version que vous venez de créer.
6. Lorsque la version de nomenclature est terminée, définissez le champ **État** sur **Validé**.  

La validité de la version est définie par le champ **Date début**.  

> [!NOTE]  
>  Sélectionnez l'option **Article** du champ **Type** pour utiliser un article des données de base article dans la nomenclature de production. Si cet article possède aussi une nomenclature de production, le champ **N° nomenclature production** est alors renseigné dans la fiche article, cette nomenclature de production est aussi prise en considération.  
>   
>  Sélectionnez l'option **Nomenclature de production** si vous souhaitez utiliser une nomenclature fantôme dans la ligne.  
>   
>  Les nomenclatures fantômes servent à structurer les produits. Ce type de nomenclature de production n'aboutit jamais à un produit fini mais est exclusivement destiné à déterminer la demande dépendante. Les nomenclatures fantômes ne possèdent pas de données de base article propres.

## <a name="quantity-calculation-formula-on-production-boms"></a>Formule de calcul de la quantité sur les nomenclatures de production  
Le calcul de la quantité tient compte des différentes dimensions également insérées dans les lignes nomenclature de production. Ces axes se rapportent à une unité de commande de l'article concerné. Les axes ainsi entrés peuvent être une longueur, une largeur, une profondeur ou un poids.  

Les colonnes Formule de calcul, Longueur, Largeur, Profondeur et Poids ne s'affichent pas car seuls quelques utilisateurs les emploient. Si vous souhaitez utiliser le calcul de la quantité, vous devez d'abord afficher ces colonnes.  

La relation entre chacun des composants est définie par la formule de calcul. Vous pouvez utiliser les formules de calcul comme suit :  

-  **Vide** - Pas de prise en compte des dimensions. (Quantité = Quantité par)  
-  **Longueur** - Quantité = Quantité par * Longueur  
-  **Longueur x Largeur** - Quantité = Quantité par * Longueur x Largeur  
-  **Longueur x Largeur x Profondeur** - Quantité = Quantité par x Longueur x Largeur x Profondeur  
-  **Poids** - Quantité = Quantité par x Poids  

### <a name="example"></a>Exemple :  
Une nomenclature de production répertorie 70 feuilles de métal dotées des dimensions suivantes : longueur = 0,20 m et largeur = 0,15 m. Les valeurs suivantes sont saisies : Formule de calcul = Longueur x Largeur, Longueur = 20, Largeur = 15, Quantité par = 70. La quantité est donnée par la valeur Quantité par x Longueur * Largeur, c'est-à-dire Quantité = 70 x 0,20 m x 0,15 m = 2,1 m2.  

## <a name="see-also"></a>Voir aussi  
[Comment créer des gammes](production-how-to-create-routings.md)   
[Paramétrage de la production](production-configure-production-processes.md)  
[Production](production-manage-manufacturing.md)    
[Planification](production-planning.md)   
[Stock](inventory-manage-inventory.md)  
[Procédure d'achat](purchasing-manage-purchasing.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

