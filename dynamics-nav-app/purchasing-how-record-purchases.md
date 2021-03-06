---
title: "Créer une facture achat et enregistrer les achats"
description: "Décrit comment acheter des articles inventaire ou service en créant et en reportant des factures ou des bons de commande."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: procurement
ms.date: 08/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d5583290925252acee6a05be29f589d057794c28
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-record-purchases"></a>Procédure : enregistrer des achats
Vous créez une facture achat ou un bon de commande pour enregistrer le coût d'achats et suivre les créances. Si vous devez contrôler un inventaire, les factures achat et les bons de commande sont également utilisés pour mettre à jour les niveaux d'inventaire de manière dynamique afin que vous puissiez réduire vos coûts d'inventaire et fournir un meilleur service au client. Le prix d'achat, notamment les frais de service, et les valeurs d'inventaire qui résultent du report des factures achat ou des bons de commande contribuent aux chiffres de profit et à d'autres KPI financiers sur votre page d'accueil.

> [!NOTE]  
>   Vous devez utiliser les commandes achat si votre processus de vente exige que vous enregistriez des réceptions partielles d'une quantité de commande, par exemple, si la quantité totale n'était pas disponible auprès du fournisseur. Si vous commercialisez des articles en les livrant directement depuis votre fournisseur auprès de votre client, vous devez également utiliser les bons de commande. Pour plus d'informations, voir [Procédure : effectuer des livraisons directes](sales-how-drop-shipment.md). Pour tous les autres aspects, les commandes achat fonctionnent de la même manière que les factures achat. La procédure suivante se base sur une facture achat. La procédure est identique pour un bon de commande.

Lorsque vous recevez les articles en inventaire, ou lorsque le service acheté est terminé, vous reportez la facture achat ou le bon de commande pour mettre à jour l'inventaire et les enregistrements financiers et pour activer le paiement au fournisseur selon les modalités de paiement. Pour plus d'informations, reportez-vous à [Effectuer des paiements](payables-make-payments.md).

> [!CAUTION]  
>   Ne reportez pas une facture achat tant que vous n'avez pas reçu les articles et que vous ne connaissez pas le coût final de l'achat, frais supplémentaires compris. Sinon, la valeur de l'inventaire et les chiffres de profit peuvent être biaisés.

Vous pouvez facilement corriger ou annuler une facture achat reportée avant de payer le fournisseur. Cela est utile si vous souhaitez corriger une erreur de saisie ou si vous souhaitez modifier l'achat assez tôt dans le processus de commande. Pour plus d'informations, reportez-vous à [Procédure : corriger ou annuler des factures achat impayées](purchasing-how-correct-cancel-unpaid-purchase-invoices.md). Si vous avez déjà payé des articles sur la facture achat reportée, vous devez créer une note de crédit achat pour inverser l'achat. Pour plus d'informations, reportez-vous à [Procédure : traiter les retours ou annulations d'achats](purchasing-how-process-purchase-returns-cancellations.md).

Les articles peuvent être de type **Stock** ou **Service**. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux articles](inventory-how-register-new-items.md). Le processus de facture achat est identique pour les deux types d'article.

Vous pouvez remplir les champs relatifs au fournisseur sur la facture achat de deux façons selon que le fournisseur est déjà enregistré ou non.

## <a name="to-create-a-purchase-invoice"></a>Pour créer une facture achat
1. Sur la page d'accueil, sélectionnez l'action **Facture achat**.  
2. Dans le champ **Fournisseur**, entrez le nom d'un fournisseur existant.

    D'autres champs de la fenêtre **Facture achat** sont désormais renseignés avec les informations standard sur le fournisseur sélectionné. Si le fournisseur n'est pas enregistré, procédez comme suit :
3. Dans le champ **Fournisseur**, entrez le nom du nouveau fournisseur.
4. Dans la boîte de dialogue d'enregistrement du nouveau fournisseur, cliquez sur le bouton **Oui**.
5. Dans la fenêtre **Sélectionnez un modèle pour un nouveau fournisseur**, sélectionnez un modèle sur lequel baser la nouvelle fiche fournisseur, puis cliquez sur le bouton **OK**.
6. Une nouvelle fiche fournisseur préremplie avec les informations sur le modèle fournisseur sélectionné s'ouvre. Le champ **Nom** est prérempli avec le nom du nouveau fournisseur que vous avez saisi sur la facture achat.
7. Renseignez les autres champs de la fiche fournisseur. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux fournisseurs](purchasing-how-register-new-vendors.md).  
8. Une fois que vous avez terminé la fiche fournisseur, cliquez sur le bouton **OK** pour revenir à la fenêtre **Facture achat**.

    Plusieurs champs de la fenêtre **Facture achat** sont renseignés avec les informations que vous avez spécifiées sur la nouvelle fiche fournisseur.
9. Renseignez les champs restants de la fenêtre **Facture achat**, selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    Vous êtes maintenant prêt à renseigner les lignes facture achat avec les articles en inventaire ou les services que vous avez achetés au fournisseur.

    > [!NOTE]  
>   Si vous avez défini des lignes achat récurrentes pour le fournisseur, par exemple un ordre de réapprovisionnement mensuel, vous pouvez insérer ces lignes sur la facture par l'intermédiaire de l'action **Extraire les lignes achat récurrentes**.
10. Dans le raccourci **Lignes**, dans le champ **N° article**, entrez le numéro d'un article en inventaire ou d'un service.
11. Dans le champ **Quantité**, indiquez le nombre d'articles à acheter.

    > [!NOTE]  
>   Pour les articles de type **Service**, la quantité est une unité de temps, telle que les heures, comme indiqué dans le champ **Code unité** de la ligne.

    Le champ **Montant ligne** est mis à jour pour indiquer la valeur du champ **Coût unitaire direct** multipliée par la valeur du champ **Quantité**.

    Le prix et le montant ligne sont affichés avec ou sans la Sales Tax en fonction de ce que vous avez sélectionné dans le champ **Prix incluant les taxes** de la fiche fournisseur.
12. Dans le champ **Montant remise facture**, entrez un montant qui doit être déduit de la valeur indiquée dans le champ **Total TTC** au bas de la facture.

    > [!NOTE]  
>   Si vous avez défini des remises facture pour le fournisseur, le pourcentage spécifié est automatiquement inséré dans le champ **% remise facture fournisseur** si les critères sont réunis, et le montant associé est inséré dans le champ **Montant remise facture**.
13. Lorsque vous recevez les articles ou services achetés, sélectionnez **Valider**.

L'achat est désormais visible dans l'inventaire et les enregistrements financiers, et le paiement fournisseur est activé. La facture achat est supprimée de la liste des factures achat et remplacée par un nouveau document dans la liste des factures achat reportées.

## <a name="see-also"></a>Voir aussi
[Procédure d'achat](purchasing-manage-purchasing.md)  
[Définition des achats](purchasing-setup-purchasing.md)  
[Procédure : Demander des devis](purchasing-how-request-quotes.md)  
[Procédure : acheter des articles pour une vente](purchasing-how-purchase-products-sale.md)  
[Procédure : enregistrer de nouveaux fournisseurs](purchasing-how-register-new-vendors.md)  
[Procédure : préparer des livraisons directes](sales-how-drop-shipment.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

