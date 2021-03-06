---
title: Configuration de la TVA sur encaissement
description: "Si vous utilisez la comptabilité basée sur la trésorerie, vous pouvez spécifier comment gérer la TVA non réalisée pour les ventes et les achats."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cash, VAT, unrealized, cash-based
ms.date: 09/08/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f5786a79e8f12bd86b3d6f7ce53e0c698b19cef4
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-set-up-unrealized-vat-for-cash-based-accounting"></a>Procédure : configurer la TVA non réalisée pour la comptabilité basée sur la trésorerie
Si vous utilisez des méthodes comptables basées sur la trésorerie, vous pouvez configurer [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] pour gérer la TVA sur encaissement.

## <a name="to-use-general-ledger-accounts-for-unrealized-vat"></a>Pour utiliser les comptes GL pour la TVA non réalisée
Vous pouvez choisir de calculer et de reporter les montants de TVA sur un compte du grand livre temporaire lorsqu'une facture est reportée, puis de les reporter sur le compte du grand livre correct et de les inclure dans les relevés fiscaux lorsque le paiement réel de la facture est reporté. Avant de pouvoir le faire, vous devez finaliser la configuration du report TVA.

Pour utiliser les comptes pour la TVA non réalisée, procédez comme suit :
1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche") et entrez **Paramètres comptabilité**. 
2. Sur la page **Paramètres comptabilité**, sous le raccourci **Général**, sélectionnez **Afficher plus**, puis activez la case à cocher **TVA sur encaissement**.
3. Fermez la page.
4. Sélectionnez l'icône **Page ou état pour la recherche** ![Page ou état pour la recherche](media/ui-search/search_small.png "Icône Page ou état pour la recherche") et entrez **Paramètres compta. TVA**. 
5. Sur la page **Paramètres compta. TVA**, sélectionnez le groupe comptabilisation TVA, puis sélectionnez **Modifier**. 
6. Dans le champ **Type TVA sur encaissement**, choisissez une option pour spécifier comment ventiler des paiements sur le montant de la facture (hors TVA) et le montant TVA, et comment transférer les montants TVA du compte TVA sur encaissement vers le compte réalisée. Le tableau suivant décrit les options.

| Option | Description |
| --- | --- |
| Vide | Sélectionnez cette option si vous ne souhaitez pas utiliser la fonction TVA non réalisée. |
| Pourcentage | Les paiements couvrent à la fois la TVA et le montant de la facture proportionnellement au pourcentage de paiement du total de la facture. Le montant de TVA payé est transféré du compte TVA non réalisée vers le compte TVA réalisée. |
| Premier | Les paiements couvrent d'abord la TVA puis le montant de la facture. Dans ce cas, le montant transféré du compte TVA non réalisée vers le compte TVA est égal au montant du paiement jusqu'à ce que la TVA soit intégralement payée. |
| Dernier | Les paiements couvrent d'abord le montant de la facture puis la TVA. Dans ce cas, aucun montant n'est transféré du compte TVA non réalisée vers le compte TVA jusqu'à ce que le montant total de la facture, hors TVA, soit payé. |
| Premier (Payé entièrement) | Les paiements couvrent d'abord la TVA (comme pour _Premier_), mais aucun montant n'est transféré vers le compte TVA jusqu'à ce que le montant total de la TVA soit payé. |
| Dernier (Payé entièrement) | Les paiements couvrent d'abord le montant de la facture (comme pour _Dernier_), mais aucun montant n'est transféré sur le compte TVA jusqu'à ce que le montant total de la TVA soit payé. |

6. Dans le champ **Cpte TVA/encaissement vente**, choisissez le compte de la TVA sur encaissement vente.

    > [!NOTE]  
>   Le montant de la TVA est reporté sur ce compte jusqu'à ce que le paiement de la facture soit reporté. Le montant est alors transféré sur le compte pour la TVA vente.
7. Dans le champ **Cpte TVA/décaissement achat**, entrez le compte général de la TVA sur décaissement achat.

    > [!NOTE]  
>   Le montant de la TVA est reporté sur ce compte jusqu'à ce que le paiement de la facture soit reporté. Le montant est alors transféré sur le compte pour la TVA vente.

## <a name="see-also"></a>Voir aussi
[Configuration de la TVA](finance-setup-vat.md)
