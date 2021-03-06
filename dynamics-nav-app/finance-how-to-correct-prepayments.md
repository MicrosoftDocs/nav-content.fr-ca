---
title: "Procédure : corriger des paiements anticipés"
description: "Vous pouvez apporter une correction à une commande après avoir reporté une facture paiement anticipé pour la commande. Vous pouvez ajouter de nouvelles lignes à une commande après avoir émis un paiement anticipé, puis vous pouvez reporter une autre facture paiement anticipé, mais vous ne pouvez pas supprimer une ligne d'une commande après avoir facturé un paiement anticipé pour la ligne."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c39223940880514f9a59eae96e88182e19db2b5e
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-correct-prepayments"></a>Procédure : corriger des acomptes
Vous pouvez apporter une correction à une commande après avoir reporté une facture paiement anticipé pour la commande. Vous pouvez ajouter de nouvelles lignes à une commande après avoir émis un paiement anticipé, puis vous pouvez reporter une autre facture paiement anticipé, mais vous ne pouvez pas supprimer une ligne d'une commande après avoir facturé un paiement anticipé pour la ligne.  

## <a name="to-correct-a-prepayment"></a>Pour corriger un paiement anticipé
La procédure suivante explique comment émettre une note de crédit paiement anticipé pour annuler tous les paiements anticipés facturés pour un document de vente.  
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Commandes vente**, puis sélectionnez le lien connexe.  
2. Ouvrez le document de vente approprié.
3. Choisissez l'action **Paiement anticipé**, puis l'action **Reporter note de crédit paiement anticipé** ou **Reporter et imprimer note de crédit paiement anticipé**.  
4. Dans la fenêtre **Note de crédit vente**, continuez à corriger les écritures appropriées, comme pour toute note de crédit vente. Pour plus d'informations, reportez-vous à [Procédure : traiter les retours ou annulations de ventes](sales-how-process-sales-returns-cancellations.md).     

    > [!NOTE]  
    > Pour réduire le montant dans le champ **Montant ligne**, vous devez commencer par augmenter le pourcentage de paiement anticipé sur la ligne afin que la valeur du champ **Montant ligne paiement anticipé** ne soit pas réduite au point d'être inférieure à la valeur du champ **Fact. montant paiement anticipé**.

5. Pour créer une facture paiement anticipé pour les nouvelles lignes dans la note de crédit vente, sélectionnez l'action **Paiement anticipé**, puis l'action **Reporter facture paiement anticipé** ou **Reporter et imprimer facture paiement anticipé**.  
6. Pour émettre une autre facture paiement anticipé, augmentez le montant de paiement anticipé sur une ou plusieurs lignes, puis reportez la facture paiement anticipé. Une nouvelle facture est créée pour la différence entre les montants de paiement anticipé facturés et les nouveaux montants de paiement anticipé.  

## <a name="see-also"></a>Voir aussi  
[Facturation de paiements anticipés](finance-invoice-prepayments.md)  
[Procédure pas à pas : configuration et facturation d'acomptes](walkthrough-setting-up-and-invoicing-sales-prepayments.md)  
[Finance](finance.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

