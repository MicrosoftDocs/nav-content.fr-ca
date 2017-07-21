<properties
                pageTitle="Procédure : Réévaluer l'inventaire | Dynamics NAV"
                description="Décrit comment réévaluer ou amortir la valeur d'un ou de plusieurs articles en inventaire en reportant leur valeur calculée actuelle."
                services="project-madeira"
                documentationCenter=""
                authors="SorenGP"
/>
<tags
    ms.service="project-madeira"
    ms.topic="article"
    ms.devlang="na"
    ms.tgt_pltfrm="na"
    ms.workload="na"
    ms.date="11/07/2016"
    ms.author="SorenGP" />


# <a name="how-to-revalue-inventory"></a>Procédure : réévaluer l'inventaire   
Pour réévaluer ou amortir un article ou une écriture article spécifique, vous devez utiliser le journal réévaluation.

## <a name="to-revalue-inventory"></a>Pour réévaluer l'inventaire
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuille réévaluation**, puis sélectionnez le lien connexe.
2. Choisissez l'action **Calculer valeur stock**.
3. Dans la fenêtre **Calculer valeur stock**, renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.
4. Cliquez sur le bouton **OK**.
5. Sur chaque ligne de la fenêtre **Feuille réévaluation**, indiquez le nouveau coût unitaire dans le champ **Coût unitaire (réévalué)**. Vous pouvez aussi indiquer le nouveau montant total dans le champ **Valeur stock (réévaluée)**.

    Les champs appropriés sont automatiquement mis à jour. Remarque : le champ **Montant** affiche la modification réelle de la valeur du stock pour l'écriture comptable article sélectionnée. Il calcule la différence entre les champs **Valeur stock (calculée)** et **Valeur stock (réévaluée)**.

6. Lorsque vous avez renseigné toutes les lignes de la feuille réévaluation, choisissez l'action **Valider**.

Les nouvelles écritures valeur sont alors créées pour refléter les appréciations que vous avez reportées. Vous pouvez visualiser les nouvelles valeurs dans les fiches article concernées.

## <a name="see-also"></a>Voir aussi
[Gestion du stock](inventory-manage-inventory.md)  
[Gestion des ventes](sales-manage-sales.md)  
[Gestion des achats](purchasing-manage-purchasing.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

