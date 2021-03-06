---
title: "Procédure : transférer les écritures GL vers les écritures de coûts"
description: "Vous pouvez transférer les écritures vers les écritures de coûts."
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
ms.openlocfilehash: b7a78fb1023e8b664fd866eb1a8b5e42ff0de265
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-transfer-general-ledger-entries-to-cost-entries"></a>Comment transférer les écritures vers les écritures de coûts
Vous pouvez transférer les écritures vers les écritures de coûts.  

Avant d'exécuter le transfert des écritures vers des écritures de coûts, vous devez vous y préparer pour éviter tout report manuel de correction.  

## <a name="to-prepare-the-transfer"></a>Pour préparer le transfert  

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Configuration de la comptabilité analytique**, puis sélectionnez le lien associé.  
2.  Dans la fenêtre **Configuration de la comptabilité analytique**, vérifiez que le champ **Date début pour transfert grand livre** est défini sur la valeur appropriée.  
3.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Plan comptable des types de coûts**, puis sélectionnez le lien associé.  
4.  Dans la fenêtre **Fiche type de coût**, vérifiez que le champ **Plage compte du grand livre** est lié correctement de sorte que chaque type de coût récupère les écritures du grand livre.  
5.  Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Plan comptable**, puis sélectionnez le lien connexe.  
6.  Pour chaque compte GL approprié, dans la fenêtre **Fiche compte GL**, vérifiez que le champ **N° type coût** est lié correctement à un type de coût. Pour plus d'informations, voir [Définition de la relation entre les types de coûts et les comptes généraux](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md).  
7.  Vérifiez que toutes les écritures GL comprennent des valeurs de dimension correspondant à un centre de coûts et à un objet de coûts.  

## <a name="to-transfer-general-ledger-entries-to-cost-entries"></a>Pour transférer les écritures vers les écritures de coûts  
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Transférer les écritures vers CA**, puis sélectionnez le lien associé.  
2.  Cliquez sur le bouton **Oui** pour démarrer le transfert. Le processus transfère toutes les écritures qui n'ont pas encore été transférées.  

    Lors du transfert, le processus crée des connexions dans les écritures des tables **Écriture de coûts** et **Registre de coûts**. Cela permet d'identifier l'origine des écritures de coûts.  

## <a name="see-also"></a>Voir aussi  
 [Critères de transfert des écritures comptables vers les écritures de coûts](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md)   
 [Transfert automatique et écritures combinées](finance-automatic-transfer-combined-entries.md)   
 [Résultats du transfert](finance-results-of-the-transfer.md)   
 [Transfert et report des écritures de coûts](finance-transfer-and-post-cost-entries.md)   
 [Définition de la relation entre les types de coûts et les comptes généraux](finance-defining-the-relationship-between-cost-types-and-general-ledger-accounts.md)   

