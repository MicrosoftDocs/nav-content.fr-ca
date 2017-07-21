---
title: "Procédure : traiter les retours ou annulations de ventes"
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
ms.openlocfilehash: 92b65379f2ec633712a2b2c0f06615c6de61cc6e
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-sales-returns-or-cancellations"></a>Procédure : traiter les retours ou annulations de ventes
Si votre client souhaite retourner ou obtenir un remboursement pour des articles, ou encore annuler des services, que vous lui avez vendus et pour lesquels vous avez reçu un paiement, vous devez créer et reporter une note de crédit vente qui indique la modification demandée. Pour inclure les informations de facture vente correctes, vous pouvez créer la note de crédit vente à partir de la facture vente reportée ou utiliser la fonction de copie.

Outre la facture vente reportée d'origine, vous pouvez affecter la note de crédit vente à d'autres documents vente, par exemple une autre facture vente reportée, parce que le client renvoie également des articles livrés avec cette facture.

Un retour ou un remboursement peut en effet se rapporter uniquement à certains des articles ou des services figurant sur la facture vente initiale. Dans ce cas, vous devez modifier les informations sur les lignes de la note de crédit vente. Lors du report de la note de crédit vente, les documents vente affectés par la modification sont inversés et un paiement de remboursement peut être créé pour le client.

Vous pouvez envoyer la note de crédit vente reportée au client pour confirmer le retour ou l'annulation et communiquer que la valeur associée sera remboursée, par exemple lorsque les articles sont renvoyés.

## <a name="to-create-a-sales-credit-memo-from-a-posted-sales-invoice"></a>Pour créer une note de crédit vente à partir d'une facture vente reportée
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Factures vente enregistrées**, puis sélectionnez le lien connexe.  
2. Dans la fenêtre **Factures vente enregistrées**, sélectionnez la facture vente validée que vous souhaitez contrepasser, puis sélectionnez l'action **Créer un avoir correctif**.

    La plupart des champs de l'en-tête de la note de crédit vente sont renseignés avec les informations de la facture vente reportée. Vous pouvez modifier tous les champs, par exemple avec de nouvelles informations qui reflètent l'entente de retour.
3. Modifiez les informations des lignes en fonction de l'entente, par exemple le nombre d'articles retournés ou le montant à rembourser.
4. Sélectionnez l'action **Lettrer écritures**.
5. Dans la fenêtre **Lettrer écritures client**, sélectionnez la ligne contenant le document vente validé auquel vous souhaitez lettrer l'avoir vente, puis sélectionnez l'action **ID lettrage**.

    Le numéro de l'avoir vente est inséré dans le champ **ID lettrage**.  
6. Dans le champ **Montant à lettrer**, entrez le montant à lettrer s'il est inférieur au montant initial.

    Au bas de la fenêtre **Lettrer écritures client**, vous pouvez afficher le montant total à lettrer pour contrepasser toutes les écritures concernées, à savoir lorsque la valeur du champ **Solde** est égale à zéro.  
7. Cliquez sur le bouton **OK**. Lorsque vous reportez la note de crédit vente, elle est affectée aux documents vente reportés spécifiés.

    Lorsque vous avez créé ou modifié les lignes note de crédit vente nécessaires et qu'une ou plusieurs affectations sont spécifiées, vous pouvez procéder au report de la note de crédit vente.
8. Sélectionnez l'action **Valider et envoyer**.

La boîte de dialogue **Valider et envoyer la confirmation** s'ouvre et indique le mode d'envoi par défaut du client. Vous pouvez modifier le mode d'envoi en cliquant sur le bouton de recherche pour le champ **Envoyer le document à**. Pour plus d'informations, reportez vous à [Procédure : configurer des profils d'envoi de documents](sales-how-setup-document-send-profiles.md).

Les documents vente reportés auxquels vous avez affecté la note de crédit sont à présent inversés, et un remboursement peut être créé pour le client. La note de crédit vente est supprimée et remplacée par un nouveau document dans la liste des notes de crédit vente reportées.

## <a name="to-create-a-sales-credit-memo-from-scratch"></a>Pour créer une note de crédit vente à partir de zéro
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Factures vente enregistrées**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau** pour ouvrir un nouvel avoir vente vierge.
3. Dans le champ **Client**, entrez le nom d'un client existant.
4. Sélectionnez l'action **Copier document**.
5. Dans la fenêtre **Extraire document vente**, dans le champ **Type document**, sélectionnez **Facture enregistrée**.
6. Sélectionnez le champ **N° document** pour ouvrir la fenêtre **Factures vente enregistrées**, puis sélectionnez la facture vente validée qui contient les lignes que vous souhaitez contrepasser.
7. Activez la case à cocher **Recalculer lignes** si vous souhaitez que les lignes facture vente validées copiées soient mises à jour avec les modifications apportées au prix article et au coût unitaire depuis la validation de la facture.
8. Cliquez sur le bouton **OK**. Les lignes facture copiées sont insérées dans la note de crédit vente.
9. Remplissez la note de crédit vente en vous reportant à la section « Pour créer une note de crédit vente à partir d'une facture vente reportée » de cette rubrique.

## <a name="see-also"></a>Voir aussi  
[Gestion des ventes](sales-manage-sales.md)  
[Configuration des ventes](sales-setup-sales.md)  
[Procédure : envoyer des documents par e-mail](ui-how-send-documents-email.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

