---
title: Importer les transactions de paie
description: "Pour gérer les paies, vous importez et reportez des transactions financières de votre fournisseur de paie dans le grand livre, en utilisant une extension de paie telle que Ceridian ou Quickbooks."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Ceridian, Quickbooks, salary
ms.date: 06/16/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 675a63c7862854ef3f8e2ca3d37dd3f2e290cf29
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-import-payroll-transactions"></a>Procédure d'importation de transactions de paie 
Pour tenir compte des paiements des salaires et des transactions associées, vous devez importer et reporter des transactions financières effectuées par votre fournisseur de paie dans le grand livre. Pour cela, vous devez commencer par importer un fichier que vous recevez du fournisseur de paie dans la fenêtre **Feuille comptabilité**. Vous devez ensuite mapper les comptes externes du fichier de paie aux comptes généraux appropriés. Enfin, vous devez reporter les transactions de paie en fonction du mappage de compte.

> [!NOTE]  
>   Pour utiliser cette fonctionnalité, une extension pour l'importation de la paie doit être installée et activée. Les extensions Salaire de Ceridian et Importer le fichier de paie de Quickbooks sont préinstallées dans [!INCLUDE[d365fin](includes/d365fin_md.md)]. Pour plus d'informations, voir [Personnalisation de [!INCLUDE[d365fin](includes/d365fin_md.md)] à l'aide des extensions](ui-extensions.md).

## <a name="to-import-a-payroll-file"></a>Pour importer un fichier de paie
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles comptabilité**, puis sélectionnez le lien connexe.
2. Dans le nom feuille comptabilité pertinent, sélectionnez l'action **Importer les transactions de paie**. Un guide de configuration assistée s'ouvre.
3. Suivez les étapes de la fenêtre **Importer les transactions de paie**.

    > [!TIP]  
>   Dans l'étape à propos du mappage des enregistrements de paie externes dans les comptes généraux, les mappages que vous effectuez seront reconnus la prochaine fois que les mêmes enregistrements seront importés. Cela vous permettra d'économiser du temps car vous n'avez pas à remplir manuellement le champ **N° compte** dans le journal général à chaque importation de transactions de paie récurrentes.   

    Lorsque vous cliquez sur le bouton **OK** dans le guide de configuration assistée, la fenêtre **Feuille comptabilité** est complétée par des lignes représentant les transactions contenues dans le fichier de paie et par les comptes appropriés des champs **Compte général** en fonction des mappages effectués dans le guide.
4. Modifiez ou reportez les lignes journal comme pour toute autre transaction du journal général. Pour plus d'informations, reportez-vous à [Procédure : Valider les transactions directement vers la comptabilité](finance-how-post-transactions-directly.md).   

## <a name="see-also"></a>Voir aussi
[Finances](finance.md)  
[Personnalisation de [!INCLUDE[d365fin](includes/d365fin_md.md)] à l'aide des extensions](ui-extensions.md)  
[Utilisation de feuilles comptabilité](ui-work-general-journals.md)  

