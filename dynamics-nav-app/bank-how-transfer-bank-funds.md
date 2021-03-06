---
title: "Transfert de fonds à la banque"
description: "Vous pouvez transférer des montants d'un compte bancaire à un autre, y compris dans différentes devises, en reportant la transaction dans le journal général."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account transfer, multiple currencies
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 5cb652df51fc5b24088bb5cc6a41d8d3f067cfd4
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-transfer-bank-funds"></a>Procédure : Transfert de fonds à la banque
Vous pouvez avoir à transférer un montant d'un compte bancaire à un autre. Pour cela, vous devez reporter une transaction dans le journal général. La tâche varie selon que les comptes bancaires utilisent la même devise ou des devises différentes.

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a>Pour reporter un transfert entre comptes bancaires avec le même code devise
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuille comptabilité**, puis sélectionnez le lien connexe.
2. Dans une ligne journal, renseignez les champs **Date de report** et **N° document** .
3. Cliquez sur le champ **Type compte**, sélectionnez le **Compte bancaire**.
4. Dans le champ **N° compte**, sélectionnez le compte bancaire à partir duquel vous souhaitez transférer les fonds.
5. Dans le champ **Montant**, entrez le total à transférer.
6. Dans le champ **Type compte contrepartie**, sélectionnez **Compte bancaire**.
7. Dans le champ **N° compte contrepartie**, sélectionnez le compte bancaire à partir duquel vous souhaitez transférer les fonds.
8. Reportez le journal.

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a>Pour reporter des transferts entre comptes bancaires dotés de codes devise différents
Pour transférer des fonds entre des comptes bancaires qui utilisent des devises différentes, vous devez reporter deux lignes journal général.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuille comptabilité**, puis sélectionnez le lien connexe.
2. Créez deux lignes journal, et renseignez les champs **Date de report** et **N° document**.
3. Sur la première ligne feuille, dans le champ **Type**, sélectionnez **Compte bancaire**.
4. Dans le champ **N° compte**, sélectionnez le compte bancaire à partir duquel vous souhaitez transférer les fonds.
5. Dans le champ **Montant**, saisissez le montant dans la devise du compte bancaire. Entrez les montants de crédit précédés du signe moins. Entrez les montants de débit sans signe moins.
6. Dans le champ **Type compte contrepartie**, sélectionnez **Compte bancaire**.
7. Dans le champ **N° compte contrepartie**, sélectionnez le compte bancaire à partir duquel vous souhaitez transférer les fonds.
8. Sur la seconde ligne feuille, dans le champ **Type**, sélectionnez **Compte bancaire**.
9. Dans le champ **N° compte**, sélectionnez le compte bancaire à partir duquel vous souhaitez transférer les fonds.
10. Dans le champ **Montant**, saisissez le montant dans la devise du compte bancaire. Entrez les montants de crédit précédés du signe moins. Entrez les montants de débit sans signe moins.
11. Dans le champ **Type compte contrepartie**, sélectionnez **Compte bancaire**.  
12. Dans le champ **N° compte contrepartie**, sélectionnez le compte bancaire à partir duquel vous souhaitez transférer les fonds.

    > [!NOTE]  
>   Si les taux de change utilisés dans la feuille sont différents des taux de change qui s'affichent dans la fenêtre **Taux de change devise**, entrez alors une troisième ligne pour les pertes ou gains liés au taux de change. Entrez **Compte général** dans le champ **Type compte**. Entrez le numéro de compte du grand livre pour les gains ou les pertes liés au taux de change dans le champ **N° compte**. Saisissez les gains ou les pertes liés au taux de change dans le champ **Montant** avec ou sans signe moins pour les crédits et les débits, respectivement.
13. Reportez le journal.

## <a name="see-also"></a>Voir aussi
[Gestion des comptes bancaires](bank-manage-bank-accounts.md)  
[Paramétrage des opérations bancaires](bank-setup-banking.md)  
[Utilisation de feuilles comptabilité](ui-work-general-journals.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

