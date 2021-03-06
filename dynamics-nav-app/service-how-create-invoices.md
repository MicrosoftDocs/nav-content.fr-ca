---
title: "Créer des factures ou des notes de crédit pour les services"
description: "Découvrez comment créer des factures, afin d'être payé pour votre service."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/22/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8c575cca9e898b31e29cdb86079e56097679b48d
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-service-invoices-or-credit-memos"></a>Procédure : créer des notes de crédit ou des factures service
La simplicité de facturation des commandes service est une fonctionnalité clé de [!INCLUDE[d365fin](includes/d365fin_md.md)]. Vous pouvez envoyer une facture à vos clients à tout moment ou créer des factures périodiquement.  
  
La fenêtre **Contrat de service** permet de créer une facture directement. Vous pouvez aussi configurer votre système afin qu'un technicien de service sur le terrain puisse créer une facture service qui est non liée à un contrat ou une commande.  

## <a name="to-invoice-a-service-contract-from-the-service-contract-page"></a>Pour facturer un contrat de service à partir de la page Contrat de service   
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Créer factures contrat service**, puis sélectionnez le lien associé.  
2. Définissez les filtres que vous souhaitez appliquer.  
3. Dans le champ **Date de report**, entrez la date à utiliser comme date de report sur les factures service.  
4. Dans le champ **Date facturation**, saisissez la date limite de facturation des contrats. Le traitement en lot inclut les contrats dont la prochaine date de facturation est antérieure à cette date.  
5. Dans le champ **Action**, sélectionnez **Créer factures**.  
6. Sélectionnez **OK** pour créer les factures service.  
  
  > [!NOTE]  
  >  Vous ne pouvez pas créer de factures service pour le contrat de service lorsque la valeur du champ **Changer état** est définie sur **Ouvert**.  
  
## <a name="to-post-an-invoice-from-a-service-order"></a>Pour reporter une facture à partir d'une commande service  
La procédure suivante décrit comment définir la partie du service que vous allez facturer au client.  

1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Commandes de service**, puis sélectionnez le lien associé.  
2. Sélectionnez la commande service à facturer, puis ouvrez la fiche de commande.  
3. Choisissez l'action **Lignes service**.  
4. Recherchez les écritures requises, puis spécifiez les quantités pour lesquelles vous allez facturer le client dans le champ **Qté à facturer**.  
  
   > [!NOTE]  
   >  Vous pouvez facturer le client pour le service enregistré soit entièrement, soit partiellement. Si vous décidez de facturer entièrement le client, la valeur renseignée dans le champ **Qté à facturer** doit être égale à celle renseignée dans le champ **Quantité**. Vous pouvez reporter une facture entière avec une livraison entière et vous pouvez reporter une facture entière pour une livraison entière déjà reportée qui n'avait pas encore été facturée ni consommée précédemment.  
   >   
   >  Lorsque vous reportez une facture partielle, vous pouvez spécifier la quantité à facturer de deux façons. Si vous comptez valider le service avec l'option **Livrer et facturer**, la valeur renseignée dans le champ **Qté à facturer** doit être égale à celle renseignée dans le champ **Qté à expédier**. Si vous voulez facturer une expédition déjà validée, la quantité à facturer ne peut pas être supérieure à la valeur renseignée dans le champ **Qté expédiée**.  
  
5. Sélectionnez **Reporter**, puis **Facturer** ou **Livrer et facturer**. Pour plus d'informations sur ces options, voir [report dans la Gestion des services](service-service-posting.md).  
  
 La ligne service que vous avez sélectionnée est reportée. Vous pouvez valider plusieurs lignes service en même temps en les sélectionnant et en choisissant **Valider**. Si vous procédez de la sorte, assurez-vous que vous avez entré toutes les informations nécessaires dans les lignes que vous voulez reporter.  
  
 Lorsque vous validez la commande avec l'option **Facturer**, une facture service validée est générée ainsi que les écritures comptables correspondantes et les champs appropriés sont mis à jour dans les lignes service de la commande. En outre, les documents livraison reportés précédemment sont mis à jour avec les quantités facturées. Si vous sélectionnez l'option de validation **Livrer et facturer**, une expédition validée est également générée.

## <a name="to-create-a-service-invoice-manually"></a>Pour créer une facture service manuellement  
Typiquement, après avoir validé une facture service avec l'option **Facturer** ou **Livrer et facturer**, une facture service validée est crée automatiquement. Toutefois, il se peut que vous deviez émettre une facture qui est non liée à un contrat de service ou à une facture service. Cette procédure explique comment émettre une facture au moment où le client reçoit le service.  

1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Factures de service**, puis sélectionnez le lien associé.  
2. Créez une facture service.  
3. Renseignez le champ **N°** .  
  
    > [!NOTE]  
    >  Si vous avez configuré une souche de numéros pour les factures service dans la fenêtre **Paramètres Gestion des services**, vous pouvez appuyer sur Entrée pour sélectionner le numéro de facture service suivant disponible.  
  
4. Dans le champ **N° client**, entrez le numéro d'un client. Sélectionnez le client approprié dans la liste.  
  
    Les champs de client sont automatiquement renseignés avec les informations de la fiche **Client**.  
  
5. Entrez une date dans le champ **Date comptabilisation**. Cette date est affichée sur les écritures reportées. Ce champ est renseigné avec la date du jour mais vous pouvez la modifier manuellement.  
6. Renseignez le champ **Date document**. La date que vous entrez apparaît sur la facture imprimée et est utilisée pour calculer la date d'échéance.  
7. Renseignez les lignes service de la facture. Renseignez les champs **Type**, **N°**, et **Quantité** pour enregistrer des articles, des ressources et des coûts utilisés pour la maintenance. 

## <a name="to-invoice-posted-shipment-lines"></a>Pour facturer des lignes livraison reportées  
Il se peut que vous deviez créer une facture service pour le service qui a déjà été livré, à partir d'une ou de plusieurs commandes service, mais pas encore facturé ni consommé. Vous pouvez renseigner les lignes facture automatiquement avec les lignes livraison reportées sélectionnées pour un client spécifique.  

1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Factures de service**, puis sélectionnez le lien associé.  
2. Renseignez les champs de la ligne selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] 
3. Créez des lignes facture pour les services livrés mais non facturés. Vous pouvez également utiliser l'action **Extraire lignes livraison** pour ajouter des lignes livraison reportées à la facture.  
4. Reportez la facture service.  
  
 La facture service reportée et les écritures correspondantes sont créées. Les documents livraison reportés précédemment sont mis à jour avec les quantités facturées et les quantités appropriées des lignes service des ordres origine.  

## <a name="to-create-a-combined-invoice"></a>Pour créer une facture regroupée  
Vous pouvez facturer le client pour les services fournis sur différentes commandes service. Des lignes facture sont créées pour des articles, des heures ou des coûts ressource qui ont déjà été livrés à partir de différentes commandes service mais non encore facturés.  

1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Factures de service**, puis sélectionnez le lien associé.  
2. Renseignez les champs de la ligne selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. Choisissez l'action **Extraire lignes livraison**. La page **Extraire lignes livraison service** affiche toutes les lignes livrées mais non facturées pour le client.  
4. Choisissez les lignes du service à facturer, puis choisissez **OK** pour ajouter les lignes livraison service à la facture.  

## <a name="to-create-a-service-credit-memo"></a>Pour créer une note de crédit service  
Un document note de crédit service est typiquement utilisé lorsqu'un client retourne un article, mais il peut également être utilisé pour offrir au client une compensation ou pour corriger une facture erronée.  

1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Notes de crédit service**, puis sélectionnez le lien associé.  
2. Renseignez les champs de la ligne selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Les champs **Date de report** et **Date document** affichent la date de travail. Si nécessaire, vous pouvez la modifier.    
4. Sur les lignes note de crédit, entrez les informations relatives aux articles retournés ou retirés, ou à la compensation qui sera donnée au client.  

## <a name="see-also"></a>Voir aussi
[Procédure : reporter des factures service](service-how-to-post-service-orders.md)  
[Paramétrage de la gestion des services](service-setup-service.md)  
[Validation de service](service-service-posting.md)  

