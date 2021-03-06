---
title: Configuration du plan comptable
description: "Vous modifiez les comptes par défaut dans le plan comptable, et vous pouvez ajouter de nouveaux comptes."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: COA, cha of acc
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b9ed31ae8e7478f57457ad68fd69d7809f706e2a
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-or-changing-the-chart-of-accounts"></a>Configuration ou modification du plan comptable
Le plan comptable affiche les comptes généraux qui stockent vos données financières. [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] inclut un plan comptable standard prêt à prendre en charge votre société.
Cependant, vous pouvez modifier les comptes par défaut, et vous pouvez ajouter de nouveaux comptes.  

## <a name="adding-or-changing-accounts"></a>Ajout ou modification de comptes
À partir du plan comptable, vous pouvez ouvrir chaque compte du grand livre et ajouter ou modifier des paramètres.

> [!NOTE]  
>   Vous pouvez supprimer un compte GL. Toutefois, avant que de le supprimer, les conditions suivantes doivent être réunies :  

* Le solde du compte doit être nul.  
* Le champ **Autoriser suppr. cpte gén. av.** doit être défini dans la fenêtre **Paramètres comptabilité**, et le compte ne doit pas comporter d'écritures comptables à cette date ou après celle-ci.  
* Si le champ **Vérifier activité cpte général** de la fenêtre **Paramètres comptabilité** est sélectionné, le compte ne doit pas être utilisé dans les groupes comptabilisation ni dans une configuration de la validation.  

[!INCLUDE[d365fin](includes/d365fin_md.md)] vous empêchera de supprimer un compte général qui stocke les données nécessaires au plan comptable.  

## <a name="see-also"></a>Voir aussi
[Les écritures comptables et le plan comptable](finance-general-ledger.md)  
[Gestion des comptes bancaires](bank-manage-bank-accounts.md)  
[Utilisation des axes analytiques](finance-dimensions.md)  
[Importation à partir d'autres systèmes financiers](upload-data.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

## 

