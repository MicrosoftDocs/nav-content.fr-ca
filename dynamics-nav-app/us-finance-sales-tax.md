---
title: "Taxe de vente et groupes de taxes aux États-Unis et au Canada"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f70a191fc8392bf1685c08c7e905ac96ba7ed069
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-tax-groups-in-the-us-and-canada"></a>Taxe de vente et groupes de taxes aux États-Unis et au Canada
Lorsque vous commencez à utiliser Dynamics NAV, vous pouvez exécuter un guide de configuration assistée afin de configurer rapidement et facilement les informations sur la taxe de vente pour votre compagnie et, éventuellement, pour vos clients et vos fournisseurs. En quelques minutes, vous êtes prêt à créer des documents vente et des documents achat pour lesquels la taxe de vente est calculée correctement.
Si vous passez à la section Ma compagnie vierge, nous vous recommandons de commencer par utiliser chacun des guides de configuration assistée, y compris celui qui concerne la taxe de vente. Si vous préférez configurer la taxe de vente par vous-même, cet article explique ce que vous devez prendre en compte.  

## <a name="tax-groups-tax-areas-and-tax-jurisdictions"></a>Groupes taxes, zones de recouvrement et autorités de recouvrement
Dans Dynamics NAV, un groupe fiscal représente un groupe de ressources ou d'articles en inventaire soumis aux mêmes conditions fiscales. Par exemple, vous pouvez configurer un groupe fiscal pour les articles soumis à la taxe et un autre pour les articles non soumis à la taxe. Vous devez affecter des codes groupe fiscal aux articles en inventaire et aux comptes du grand livre. De même, vous devez affecter des codes de région fiscale aux clients, aux emplacements et aux paramètres de votre compagnie. Le guide de configuration assistée vous aide à effectuer ces opérations.  

Chaque région fiscale correspond à un regroupement de juridictions de taxe de vente basé sur une situation géographique particulière. Par exemple, la région fiscale de Miami, Floride, comprend trois juridictions pour la taxe de vente : la ville (Miami), le comté (Dade) et la province (Floride). Dynamics NAV inclut un ensemble limité de zones de recouvrement avec une configuration par défaut, mais vous pouvez les modifier et ajouter de nouvelles zones de recouvrement.  

Si vous configurez de nouvelles zones et juridictions de recouvrement, vous devez veiller à bien remplir les champs correctement. Aux États-Unis, les états, les comtés, les villes et les localités peuvent prélever la taxe de vente. Au Canada, le gouvernemental fédéral et les provinces sont en mesure de prélever la taxe de vente. Les compagnies recueillent la taxe de vente et la versent aux autorités gouvernementales pour les produits vendus aux utilisateurs finaux. La taxe de vente peut également être facturée sur une taxe de vente existante. Par exemple, la taxe peut être calculée sur un montant facture vente qui comprend déjà la taxe imposée par d'autres autorités.  

Au Canada, les montants de taxe doivent être détaillés dans les documents concernant chaque juridiction fiscale. Jusqu'à quatre autorités de recouvrement peuvent apparaître dans un document, et les autorités dotées du même ordre d'impression sont regroupées lors de l'impression.

## <a name="tax-details"></a>Détails fiscaux
La fenêtre **USA spécifications taxe** affiche différentes combinaisons de zones de recouvrement de la Sales Tax et de groupes de taxe afin d'établir les taux de taxe. Pour chaque juridiction fiscale, nous vous recommandons de configurer un groupe fiscal pour la taxe de vente normale, un autre groupe fiscal pour les articles ou les services qui ne sont pas soumis à la taxe et un groupe fiscal supplémentaire pour chaque type d'article ou de service traité avec un taux de taxe de vente différent dans cette juridiction fiscale.  

Aux États-Unis, lorsque vous vendez à un client dans un magasin où vous n'avez pas de *situs*(ou un magasin légal dans cet état) vous ne percevez pas la Sales Tax. Pour les magasins dans lesquels vous n'avez pas de situs, assurez-vous que la valeur des champs **Taxe inférieure minimum** and **Taxe supérieure maximum** est égale à 0,00.  

## <a name="see-also"></a>Voir aussi
[Finance](finance-setup.md)  
[Configuration de la finance](finance-setup-setup-finance-setup.md)  
[Taxe sur les ventes et taxe sur les biens et les services au Canada](ca-finance-setup-tax.md)  
[Configuration simplifiée de la Sales Tax](https://madeira.microsoft.com/en-us/blog/sales-tax-setup-made-easy)  

