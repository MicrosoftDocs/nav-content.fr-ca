---
title: En savoir plus sur le grand livre et le COA
description: "Décrit le grand livre, le plan comptable, et les catégories de compte."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 348a1bcbe6908c7bfd84e99245363e733414aeae
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="understanding-the-general-ledger-and-the-coa"></a>Familiarisation avec le grand livre et les COA
Le grand livre stocke vos données financières, et le plan comptable affiche les comptes sur lesquels toutes les écritures sont reportées. [!INCLUDE[d365fin](includes/d365fin_md.md)] inclut un plan comptable standard prêt à prendre en charge votre société.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Configuration du grand livre et configuration du report général
La configuration du grand livre est la composante principale des processus financiers car elle définit comment vous reportez les données.  

Dans la fenêtre **Paramètres comptabilité**, vous spécifiez comment gérer certains problèmes comptables dans votre société, par exemple :  

* Les détails arrondissement facture  
* Les formats d'adresse  
* Rapports financiers  

De même, dans la fenêtre **Paramètres comptabilisation**, vous spécifiez comment vous souhaitez configurer les combinaisons de groupes généraux comptabilisation marché et de groupes généraux comptabilisation produit. Les groupes comptabilisation mappent des entités telles que les clients, les fournisseurs, les éléments, les ressources et les documents vente et achat dans des comptes généraux. Saisissez une ligne pour chaque combinaison de groupes de report marché et de groupes de report produit. Pour plus d'informations, voir [Paramètres du groupe comptabilisation](finance-posting-groups.md)  

## <a name="the-chart-of-accounts"></a>Le plan comptable
Le plan comptable affiche tous les comptes généraux. Vous pouvez effectuer les opérations suivantes à partir du plan comptable :  

* Afficher les rapports qui affichent les écritures et les soldes.  
* Fermez votre état des résultats.  
* Ouvrir la fiche compte du grand livre pour ajouter ou modifier des paramètres.  
* Consulter la liste des groupes de report qui effectuent les reports vers ce compte.
* Afficher les soldes débit et crédit d'un seul compte  

Vous pouvez ajouter, modifier ou supprimer des comptes généraux. Toutefois, pour éviter les différences, vous ne pouvez pas supprimer un compte du grand livre si ses données sont utilisées dans le plan comptable.  

## <a name="account-categories"></a>Catégories de compte
Vous pouvez personnaliser la structure de vos états financiers en mappant les comptes généraux aux catégories de comptes.  

La fenêtre **Catégories de compte général** affiche vos catégories et sous-catégories et les comptes généraux que leurs sont affectés. Vous pouvez créer des sous-catégories et affecter ces catégories à des comptes existants.  

Vous créez un groupe des catégories en effectuant une indentation d'autres sous-catégories sous une ligne de la fenêtre **Catégories de compte général**. Cela vous facilite l'obtention d'une vue d'ensemble, car chaque groupement affiche un solde total. Par exemple, vous pouvez créer des sous-catégories pour différents types d'actifs puis créer des groupes des catégories pour différencier les immobilisations des actifs à court terme, par exemple.  

Vous pouvez spécifier si les comptes de chaque sous-catégorie doivent être inclus dans des types spécifiques d'états. Les catégories de compte vous aident à définir la présentation de vos états financiers.  

Par exemple, le solde relevé par défaut solde est doté d'une sous-catégorie pour la trésorerie dans Actifs à court terme. Si vous souhaitez que le solde relevé tienne compte du fonds de caisse et du compte chèque, vous pouvez :  

1. Ajouter deux nouvelles sous-catégories. Une pour le fonds de caisse, et l'autre pour le compte chèque  
2. Spécifier la définition d'état supplémentaire **Comptes de trésorerie** pour ces sous-catégories.  
3. Effectuer une indentation sous la sous-catégorie **Trésorerie**.  

À la prochaine génération des tableaux d'analyse, votre relevé solde suivant affichera un solde total pour la trésorerie et deux lignes avec les soldes pour le fonds de caisse et le compte chèque.  

## <a name="see-also"></a>Voir aussi
[Finances](finance.md)  
[Configuration ou modification du plan comptable](finance-setup-chart-accounts.md)  
[Veille économique](bi.md)  

