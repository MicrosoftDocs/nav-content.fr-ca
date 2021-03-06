---
title: "Procédure : créer des itinéraires"
description: "Un itinéraire contient les données de base qui capturent les exigences du traitement correspondant à un article produit donné. Après la création d'un bon de production pour cet article, son itinéraire gouvernera la programmation des opérations comme représenté dans la fenêtre **Itinéraire bon de prod.** sous le bon de production."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 49cce1f32f1d66dc17c0d9758937541ef1baaae7
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-routings"></a>Comment créer des gammes
Les compagnies manufacturières utilisent des itinéraires pour visualiser et gérer le processus de fabrication.

L'itinéraire est la base de la programmation des processus et des capacités, de l'affectation programmée du matériel en fonction des besoins et des documents de production.  

En ce qui concerne les nomenclatures de production, les itinéraires sont affectés à l'article fini produit. Un itinéraire contient les données de base qui capturent les exigences du traitement correspondant à un article produit donné. Après la création d'un ordre de fabrication pour cet article, sa gamme gouvernera le calendrier des opérations tels que représenté dans la fenêtre **Gamme O.F.** sous l'ordre de fabrication.  

Pour pouvoir configurer un itinéraire, les éléments suivants doivent être en place :  

- Des fiches article sont créées pour les articles parents qui participent à la production. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux articles](inventory-how-register-new-items.md).
- Les ressources de production sont configurées. Pour plus d'informations, voir [Procédure : configurer des ateliers et des unités de production](production-how-to-set-up-work-and-machine-centers.md).

## <a name="to-create-a-routing"></a>Pour créer un itinéraire  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Itinéraires**, puis sélectionnez le lien associé.  
2.  Sélectionnez l'action **Nouveau**.  
3. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  Dans le champ **Type**, sélectionnez **Série** pour calculer la gamme de fabrication en fonction de la valeur de **N° opération** . .   
    Sélectionnez **Parallèle** pour calculer les opérations en fonction de la valeur de **Numéro de l'opération suivante**. .  
5.  Pour modifier la gamme, définissez le champ **Statut** sur **Création en cours** ou sur **Modification en cours**. Pour l'activer, définissez le champ **Statut** sur **Validée**.  

    Renseignez les lignes itinéraire.
6.  Dans le champ **N° opération**, entrez le numéro de la première opération \(par exemple, **10**\).  
7.  Dans le champ **Type**, sélectionnez le type de ressource utilisé, par exemple, **Centre de charge**.  
8.  Dans le champ **N°**, sélectionnez la ressource à utiliser, ou entrez\-la.  
9.  Dans le champ **Code lien gamme**, vous pouvez entrer un code permettant de lier le composant à une opération spécifique. Pour plus d'informations, voir la section « Pour créer des liens itinéraire ».
10.  Dans les champs **Temps d'exécution** et **Temps de préparation**, entrez les temps opératoires nécessaires pour exécuter l'opération.  

    > [!NOTE]  
    >  Le temps de préparation est calculé par bon de production, tandis que le temps d'exécution est calculé par article produit.  

11.  Dans le champ **Capacités simultanées** , indiquez combien d'unités de la ressource sélectionnée sont utilisées pour exécuter l'opération. Par exemple, deux personnes affectées à une opération de livraison diviseront par deux le temps d'exécution.  
12.  Poursuivez le remplissage des lignes pour toutes les opérations intervenant dans la production de l'article en question.  
13.  Pour copier des lignes à partir d'un itinéraire existant, choisissez l'action **Copier itinéraire** pour sélectionner des lignes existantes.  
14. Certifiez l'itinéraire.  
15. Vous pouvez désormais lier le nouvel itinéraire à la fiche de l'article de production concerné en renseignant le champ **N° itinéraire**. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux articles](inventory-how-register-new-items.md).  

> [!NOTE]  
>  N'oubliez pas également de recalculer le coût standard de l'article de la fiche **Article** : choisissez l'action **Production**, sélectionnez l'action **Calculer coût standard**, puis sélectionnez l'action **Tous niveaux**.  

## <a name="to-create-routing-links"></a>Pour créer des liens itinéraire
Vous pouvez créer des liens itinéraire pour lier des composantes à des opérations spécifiques afin de conserver leur relation, même si la nomenclature de production ou l'itinéraire sont modifiés. Cela simplifie également la consommation juste-à-temps des composantes, à savoir lorsque l'opération liée commence, et non quand le bon de production complet est libéré. Pour plus d'informations, voir [Procédure : consommer en aval des composants en fonction de la production réalisée](production-how-to-flush-components-according-to-operation-output.md).  

Les composants et opérations liés apparaissent dans une structure opératoire logique lorsque vous utilisez la fenêtre **Feuille production** pour la validation production et consommation, ce qui constitue un autre avantage majeur.  

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Itinéraires**, puis sélectionnez le lien associé.  
2.  Ouvrez l'itinéraire contenant les opérations que vous voulez lier.  

    Vérifiez que le statut de la gamme est **Modification en cours**.  

3.  Sur la ligne gamme appropriée, dans le champ **Code lien gamme** , sélectionnez un code.  
4.  Ajoutez ensuite plusieurs codes lien itinéraire à d'autres opérations de l'itinéraire, si nécessaire.  

    > [!NOTE]  
    >  Vous ne devez pas utiliser le même code lien itinéraire dans plusieurs opérations d'un itinéraire, car vous risquez de lier de manière incorrecte une même composante à deux opérations différentes et, de ce fait, de la consommer deux fois.  
    >   
    >  Il peut être judicieux de nommer le code lien itinéraire au terme de l'opération pour garantir que les liens itinéraire soient propres à chaque opération.

5.  Définissez le statut de la gamme sur **Validé**.  

    Les codes lien itinéraire sont désormais affectés aux opérations. Ensuite, vous devez créer le lien réel en attribuant les mêmes codes à des composants spécifiques de la nomenclature de production appropriée.  

6.  Ouvrez la **Nomenclature de production** qui contient les composantes à lier aux opérations ci-dessus. Pour plus d'informations, reportez\-vous à [Procédure : créer des nomenclatures de production](production-how-to-create-production-boms.md).
7.  Vérifiez que le statut de la nomenclature est **Modification en cours**.  
8.  Sur la ligne appropriée de nomenclature de production, dans le champ **Code lien gamme**, sélectionnez le code que vous venez d'affecter à l'opération correspondante.  
9. Ajoutez ensuite des codes lien itinéraire à d'autres composantes, selon les opérations uniques pour lesquelles ils sont utilisés.  
10. Définissez le statut de la nomenclature de production sur **Validé**.  

    > [!NOTE]  
    >  Pour activer les liens itinéraire d'un bon de production existant, vous devez actualiser le bon de production. Pour plus d'informations, voir [Procédure : créer des ordres de fabrication](production-how-to-create-production-orders.md).  

Les composantes sélectionnées seront liées aux opérations sélectionnées lorsque vous créerez ou actualiserez un bon de production à l'aide de la nomenclature de production et de l'itinéraire concernés. Ceci est visible dans la fenêtre **Composants O.F.** sous l'ordre de fabrication. Ici, vous pouvez également ajouter ou supprimer à tout moment les codes lien gamme définis.

## <a name="to-assign-personnel-tools-and-quality-measures-to-routing-operations"></a>Pour affecter des qualifications, des outils et des contrôles qualité à des opérations itinéraire.
Si vous avez besoin de personnes ayant des qualifications, un savoir-faire particulier, ou bénéficiant d'une autorisation spéciale pour une opération, vous pouvez affecter ces personnes à l'opération. En outre, vous pouvez affecter des outils et des exigences de qualité à l'opération. Cette procédure décrit l'affectation de qualifications. Les étapes sont similaires pour d'autres types d'informations sur l'opération.

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Itinéraires**, puis sélectionnez le lien associé.  
2.  Ouvrez l'itinéraire approprié.  
3.  Sur le raccourci **Lignes**, sélectionnez la ligne à traiter, puis choisissez l'action **Qualifications**.  
4.  Renseignez les champs de la fenêtre **Qualifications gamme**.  
5.  Cliquez sur le bouton **OK** pour quitter la fenêtre. Les valeurs saisies sont copiées et affectées à l'opération.    

## <a name="to-create-a-new-versions-of-a-routing"></a>Pour créer une nouvelle version d'un itinéraire  
Le principe de la version permet de gérer différentes versions d'un itinéraire. La structure d'une version d'itinéraire correspond à la structure de l'itinéraire composée d'un en-tête et de lignes version d'itinéraire. La différence de base est définie par la date début.  

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Itinéraires**, puis sélectionnez le lien associé.  
2.  Sélectionnez l'itinéraire à copier, puis choisissez l'action **Versions**.  
3. Dans la fenêtre **Versions d'itinéraire**, sélectionnez l'action **Nouveau**.
4. Renseignez les champs selon vos besoins.
5.  Dans le champ **Code version**, saisissez le numéro d'identification unique de la version. Ce champ admet n'importe quelle combinaison de chiffres et de lettres.  

    Le statut **Nouveau** est automatiquement affecté à la version que vous venez de créer.  
6.  Pour créer des lignes opération, sélectionnez la première ligne vide, puis renseignez le champ **N° opération** en fonction de la séquence des opérations.

    Les lignes opération sont triées par ordre croissant, en fonction du numéro des opérations. Afin de faciliter les modifications ultérieures, optez pour des incréments de taille adéquate. Le champ **N° opération suivante** se réfère à l'opération suivante. Vous pouvez y entrer directement le numéro de l'opération.

7. Lorsque la version d'itinéraire est terminée, définissez le champ **État** sur **Validé**.

La validité de la version est définie par le champ **Date début**.  

## <a name="see-also"></a>Voir aussi  
[Comment créer des nomenclatures de production](production-how-to-create-production-boms.md)  
[Paramétrage de la production](production-configure-production-processes.md)  
[Production](production-manage-manufacturing.md)    
[Planification](production-planning.md)   
[Stock](inventory-manage-inventory.md)  
[Procédure d'achat](purchasing-manage-purchasing.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

