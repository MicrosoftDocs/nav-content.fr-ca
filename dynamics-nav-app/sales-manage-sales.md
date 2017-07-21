---
title: Gestion des ventes
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
ms.openlocfilehash: 20e380abb2f8f598391a66e50a7ec7a1c8b15fa1
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="manage-sales"></a>Gestion des ventes
Vous créez une facture vente ou un document de vente pour enregistrer votre entente avec un client pour vendre certains produits selon certaines modalités de livraison et de paiement.

Vous devez utiliser des documents de vente si votre processus de vente requiert que vous livriez des parties d'une quantité de commande, par exemple, si la quantité totale est pas disponible d'un coup. Si vous vendez des articles en les livrant directement du fournisseur au client (livraison directe), vous devez également utiliser des documents de vente. Pour tous les autres aspects, les commandes vente fonctionnent de la même manière que les factures vente.  

Les pratiques recommandées en matière de vente et de marketing reposent toutes sur la prise de décisions appropriées au bon moment. La fonctionnalité Marketing de Dynamics NAV fournit une vue d'ensemble précise et opportune de vos informations de contact afin d'offrir des services à vos prospects de manière plus efficace et d'accroître la satisfaction de la clientèle. Pour plus d'informations, reportez-vous à [Gestion des relations](marketing-relationship-management.md).

Vous pouvez négocier avec le client en créant d'abord un devis, que vous pouvez convertir en facture vente lorsque vous êtes d'accord sur la vente. Une fois que le client a confirmé l'entente, par exemple après une procédure de devis, vous pouvez envoyer une confirmation de commande pour enregistrer votre obligation de fournir les produits comme convenu.

Lorsque vous livrez les produits, entièrement ou partiellement, vous reportez la facture vente ou le document de vente comme étant livré ou livré et facturé pour créer les écritures article et client associées dans votre système.

Dans les environnements d'entreprise où le client doit payer avant la livraison des produits vendus (par exemple la vente au détail), vous devez attendre la réception du paiement avant de fournir les produits. Dans la plupart des cas, vous traitez les paiements entrants plusieurs semaines après la livraison en affectant les paiements à leurs factures vente reportées et impayées associées. Pour plus d'informations, reportez-vous à [Procédure : rapprocher les paiements à l'aide de l'application automatique](receivables-how-reconcile-payments-auto-application.md).

Les documents de vente peuvent être envoyés sous forme de fichiers PDF joints au courriel. Le corps du message contient un extrait du document de vente, comme les produits, le montant total et un lien vers le site Paypal. Pour plus d'informations, reportez vous à [Procédure : envoyer des documents par e-mail](ui-how-send-documents-email.md).

Pour tous les processus de vente, vous pouvez incorporer un flux de travail d'approbation, par exemple, pour exiger que les ventes en grande quantité à certains clients soient approuvés par le responsable de la comptabilité. Pour plus d'informations, reportez-vous à [Utilisation des flux d'approbation](across-how-use-approval-workflows.md).

Le tableau suivant décrit une série de tâches et inclut des liens vers les rubriques qui les décrivent.

|À |Voir |
|---|----|
|Créer un devis dans lequel vous proposer des biens selon des conditions négociables avant de convertir le devis en facture vente.|[Procédure : créer des offres](sales-how-make-offers.md)|
|Créer une facture vente pour enregistrer votre entente avec un client pour vendre des produits selon certaines modalités de livraison et de paiement.|[Procédure : facturer des ventes](sales-how-invoice-sales.md)|
|Traiter un document de vente qui implique une livraison partielle ou une livraison directe.|[Procédure : vendre des produits](sales-how-sell-products.md)|
|Lier un document de vente à un bon de commande pour vendre un article qui sera livré directement de votre fournisseur à votre client.|[Procédure : effectuer des livraisons directes](sales-how-drop-shipment.md)|
|Créez une note de crédit vente pour rétablir une facture vente reportée spécifique pour indiquer quels produits sont retournés par le client et quel montant règlement vous rembourserez.|[Procédure : traiter les retours ou annulations de ventes](sales-how-process-sales-returns-cancellations.md)|
|Créer une fiche client pour chaque client auquel vous vendez des éléments.|[Procédure : enregistrer de nouveaux clients](sales-how-register-new-customers.md)|

## <a name="see-also"></a>Voir aussi  
[Configuration des ventes](sales-setup-sales.md)  
[Gestion des comptes client](receivables-manage-receivables.md)  
[Gestion des comptes fournisseur](payables-manage-payables.MD)      
[Utiliser Dynamics NAV](ui-work-product.md)  
[Fonctionnalités communes aux différents secteurs d'activité](ui-across-business-areas.md)

