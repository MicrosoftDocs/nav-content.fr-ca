---
title: "Détails de conception - périodes d'inventaire"
description: "Des transactions antidatées ou des ajustements des coûts affectent souvent les soldes et les évaluations de l'inventaire pour des périodes comptables qui peuvent être considérées comme fermées. Ceci peut avoir des effets négatifs sur la précision des rapports, notamment dans des sociétés internationales. La fonction Périodes d'inventaire permet d'éviter ces problèmes en ouvrant ou en fermant des périodes d'inventaire pour limiter le report dans une période définie."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1dd508ee887b28b1696746444145eff6f2bd7ebe
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-inventory-periods"></a>Détails de conception : périodes inventaire
Des transactions antidatées ou des ajustements des coûts affectent souvent les soldes et les évaluations de l'inventaire pour des périodes comptables qui peuvent être considérées comme fermées. Ceci peut avoir des effets négatifs sur la précision des rapports, notamment dans des sociétés internationales. La fonction Périodes d'inventaire permet d'éviter ces problèmes en ouvrant ou en fermant des périodes d'inventaire pour limiter le report dans une période définie.  

 Une période d'inventaire est une période, définie par une date de fin, pendant laquelle vous reportez des mouvements d'inventaire. Lorsque vous fermez une période d'inventaire, aucun changement de valeur ne peut être reporté dans la période fermée. Cela inclut de nouvelles validations de valeur, des validations prévues ou facturées, des modifications sur les valeurs existantes et des ajustements de coûts. Cependant, vous pouvez toujours affecter une écriture article ouverte qui se trouve dans la période fermée. Pour plus d'informations, voir [Détails de conception : traçabilité](design-details-item-application.md).  

 Pour s'assurer que toutes les écritures de transaction dans une période fermée sont finales, les conditions suivantes doivent être remplies avant qu'une période d'inventaire ne soit fermée :  

-   Toutes les écritures article sortantes de la période doivent être fermées (aucun inventaire négatif).  
-   Tous les coûts des articles pour la période doivent être ajustés.  
-   Tous les bons de production libérés et terminés dans la période doivent faire l'objet d'un ajustement des coûts.  

 Lorsque vous fermez une période d'inventaire, une écriture période d'inventaire est créée à l'aide du numéro du dernier registre d'article tombant dans la période d'inventaire. En outre, le délai, la date et le code utilisateur de l'utilisateur fermant la période sont enregistrés dans l'écriture période d'inventaire. À l'aide des informations associées au dernier registre d'article de la période précédente, vous pouvez visualiser les mouvements d'inventaire qui ont été reportés pour la période d'inventaire. Il est également possible de rouvrir des périodes d'inventaire si vous devez reporter dans une période fermée. Lorsque vous rouvrez une période d'inventaire, une écriture période d'inventaire est créée.  

## <a name="see-also"></a>Voir aussi  
 [Détails de conception : Coûts ajustés](design-details-inventory-costing.md) [Gestion des coûts ajustés](finance-manage-inventory-costs.md) [Finance](finance.md)  
 [Utilisation de Dynamics NAV](ui-work-product.md)

