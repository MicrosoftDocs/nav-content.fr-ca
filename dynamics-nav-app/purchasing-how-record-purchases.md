---
title: "Procédure : enregistrer des achats"
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 6d1933bf1e1c9236d34d429a4da84c907df13708
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-record-purchases"></a>Procédure : enregistrer des achats
Vous créez une facture achat ou un bon de commande pour enregistrer le coût d'achats et suivre les créances. Si vous devez contrôler un inventaire, les factures achat et les bons de commande sont également utilisés pour mettre à jour les niveaux d'inventaire de manière dynamique afin que vous puissiez réduire vos coûts de l'inventaire et fournir un meilleur service au client. Le prix d'achat, notamment les frais de service, et les valeurs d'inventaire qui résultent du report des factures achat ou des bons de commande contribuent aux chiffres de profit et à d'autres KPI financiers sur votre page d'accueil.

**Remarque** : vous devez utiliser les commandes achat si votre processus de vente exige que vous enregistriez des réceptions partielles d'une quantité de commande, par exemple, si la quantité totale n'était pas disponible auprès du fournisseur. Si vous vendez des articles en les livrant directement du fournisseur au client (livraison directe), vous devez également utiliser des bons de commande. Pour plus d'informations, voir [Procédure : effectuer des livraisons directes](sales-how-drop-shipment.md). Pour tous les autres aspects, les commandes achat fonctionnent de la même manière que les factures achat. La procédure suivante se base sur une facture achat. La procédure est identique pour un bon de commande.

Lorsque vous recevez les articles en inventaire, ou lorsque le service acheté est terminé, vous reportez la facture achat ou le bon de commande pour mettre à jour l'inventaire et les enregistrements financiers et pour activer le paiement au fournisseur selon les modalités de paiement. Pour plus d'informations, reportez-vous à [Exécuter des paiements](payables-make-payments.md).

**Attention** ! Ne validez pas une facture achat tant que vous n'avez pas reçu les produits et que vous ne connaissez pas le coût total de l'achat, frais supplémentaires compris. Sinon, la valeur de l'inventaire et les chiffres de profit peuvent être biaisés.

Si vous avez déjà payé des produits sur la facture achat reportée, vous devez créer une note de crédit achat pour inverser l'achat. Pour plus d'informations, reportez-vous à [Procédure : traiter les retours ou annulations d'achats](purchasing-how-process-purchase-returns-cancellations.md).

Les produits peuvent être des articles en inventaire et des services. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux produits](inventory-how-register-new-products.md). Le processus de facture achat est identique pour les deux types de produit.



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
9. Renseignez les champs restants de la fenêtre **Facture achat**, selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

    Vous êtes maintenant prêt à renseigner les lignes facture achat avec les articles inventaire ou les services que vous avez achetés au fournisseur.

    **Remarque** : si vous avez défini des lignes achat récurrentes pour le fournisseur, par exemple un ordre de réapprovisionnement mensuel, vous pouvez insérer ces lignes sur la facture par l'intermédiaire de l'action **Extraire les lignes achat récurrentes**.
10. Sur le raccourci **Lignes**, dans le champ **N° article**, saisissez le numéro d'un article en inventaire ou d'un service.
11. Dans le champ **Quantité**, indiquez le nombre d'articles à acheter.

    **Remarque** : pour les articles de type **Service**, la quantité est une unité de temps, telle que les heures, comme indiqué dans le champ **Code unité** de la ligne.

    Le champ **Montant ligne** est mis à jour pour indiquer la valeur du champ **Coût unitaire direct** multipliée par la valeur du champ **Quantité**.

    Le prix et le montant ligne sont affichés avec ou sans la Sales Tax en fonction de ce que vous avez sélectionné dans le champ **Prix incluant les taxes** de la fiche fournisseur.
12. Dans le champ **Montant remise facture**, entrez un montant qui doit être déduit de la valeur indiquée dans le champ **Total TTC** au bas de la facture.

    **Remarque** : si vous avez défini des remises facture pour le fournisseur, le pourcentage spécifié est automatiquement inséré dans le champ **% remise facture fournisseur** si les critères sont réunis, et le montant associé est inséré dans le champ **Montant remise facture**.
13. Lorsque vous recevez les articles ou services achetés, sélectionnez **Valider**.

L'achat est désormais visible dans l'inventaire et les enregistrements financiers, et le paiement fournisseur est activé. La facture achat est supprimée de la liste des factures achat et remplacée par un nouveau document dans la liste des factures achat reportées.

## <a name="see-also"></a>Voir aussi  
[Gestion des achats](purchasing-manage-purchasing.md)  
[Configuration des procédures achat](purchasing-setup-purchasing.md)  
[Procédure : acheter des produits pour une vente](purchasing-how-purchase-products-sale.md)  
[Procédure : enregistrer de nouveaux fournisseurs](purchasing-how-register-new-vendors.md)  
[Procédure : préparer des livraisons directes](sales-how-drop-shipment.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

