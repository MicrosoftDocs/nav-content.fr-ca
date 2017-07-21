---
title: Taxe de vente et taxe sur les biens et les services au Canada
author: edupont04
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c032a02b545441b927ef5c4facc9f77731f37ab7
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-goods-and-services-tax-in-canada"></a>Taxe de vente et taxe sur les biens et les services au Canada
Au Canada, si un fournisseur n'a pas de présence commerciale dans la province dans laquelle les achats sont effectués, le fournisseur facture la taxe sur les produits et services (TPS) ou la taxe de vente harmonisée (HST) uniquement. Toutefois, si la province applique une taxe de vente provinciale (PST), l'acheteur doit tout de même calculer le montant de la PST et le payer directement à la province. Lorsqu'un code région fiscale provinciale est sélectionné, Dynamics NAV l'utilise pour calculer la PST et la reporter de sorte que l'impôt à payer apparaisse à la fois dans le grand livre et dans les enregistrements d'écriture TVA. Par conséquent, le code région fiscale sélectionné ici doit uniquement inclure la PST et non la GST.  
Pour plus d'informations de la taxe sur les ventes, reportez-vous à [Taxe sur les ventes et groupes de taxes aux États-Unis et au Canada](us-finance-setup-sales-tax.md).  

## <a name="submitting-the-gsthst-file"></a>Envoi du fichier GST/HST
Les informations sur les taxes dans les documents achat permettent de générer un transfert de fichier GST/HST par Internet, fichier que vous devez transmettre aux autorités fiscales. Ce champ inclut la taxe sur les biens et les services (GST) et la taxe de vente harmonisée (HST). Le fichier est créé dans un format de fichier .tax, qui peut être transféré via Internet.  

## <a name="see-also"></a>Voir aussi
[Finance](finance-setup.md)  
[Configuration de la finance](finance-setup-setup-finance-setup.md)  
[Taxe sur les ventes et groupes de taxes aux États-Unis et au Canada](us-finance-setup-sales-tax.md)

