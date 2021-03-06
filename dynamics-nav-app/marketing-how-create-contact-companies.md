---
title: "Création de sociétés contact"
description: "Décrit comment créer un contact pour chaque nouvelle compagnie ou compagnie prospect avec laquelle vous collaborez ou entretenez des relations."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 02269adb44c5b036140aa9c920c4ffb5a64e13c1
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-contact-companies"></a>Procédure : créer des compagnies contact
Vous pouvez créer un contact pour chaque nouvelle compagnie avec laquelle vous êtes en contact, par exemple un client, un fournisseur, un prospect, une banque, un cabinet d'avocats, un consultant, et ainsi de suite.

Il existe deux méthodes permettant de créer un contact : à partir de zéro ou à partir d'un client, d'un fournisseur ou d'un compte bancaire existant.

Avant de créer un contact, vous pouvez vérifier les paramètres dans la fenêtre **Paramètres Marketing**. Pour plus d'informations, voir [Paramétrage de la Gestion des relations](marketing-setup-marketing.md).

## <a name="create-a-company-contact-from-scratch"></a>Créer un contact compagnie à partir de zéro
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Contacts**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau**.
3. Dans le champ **N°**, saisissez le numéro du contact.

    Si vous avez configuré une souche de numéros pour les contacts dans la fenêtre **Paramètres Marketing**, appuyez sur la touche Entrée pour sélectionner le numéro de contact suivant.  
4. Définissez **Type** à **Société**.
5. Renseignez les autres champs selon vos besoins.

## <a name="to-create-a-company-contact-from-a-customer-vendor-or-bank-account"></a>Pour créer un contact compagnie à partir d'un client, d'un fournisseur ou d'un compte bancaire
Si vous avez configuré plusieurs clients, fournisseurs et comptes bancaires, vous pouvez créer des contacts sur la base des données existantes. Lorsque vous créez un contact de cette façon, les informations de contact sont synchronisées avec les informations du client, du fournisseur ou du compte bancaire.

> [!NOTE]  
>   Avant de créer des sociétés contact de cette manière, vous devez spécifier un code relation d'affaires pour les clients, les fournisseurs, ainsi que des comptes bancaires dans la fenêtre **Paramètres marketing**. Si vous devez créer des contacts à partir de comptes bancaires, vous devez également spécifier des souches de numéros pour les comptes bancaires dans la fenêtre **Paramètres comptabilité**.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez l'un des choix suivants, selon l'élément à partir duquel vous souhaitez créer des contacts, puis sélectionnez le lien connexe.
   * **Créer contacts à partir des clients**
   * **Créer contacts à partir des fournisseurs**
   * **Créer contacts à partir des cptes banc**
2. Dans la fenêtre de traitement par lots qui s'affiche, dans la section **Client**, **Fournisseur** ou **Compte bancaire**, définissez des filtres si vous souhaitez créer des contacts à partir de clients, de fournisseurs ou de comptes bancaires spécifiques.
3. Pour démarrer la création de contacts, cliquez sur le bouton **OK**.

    Les numéros de contact suivants de la série de numéros sont affectés aux nouveaux contacts. La relation d'affaires des fournisseurs qui est spécifiée dans la fenêtre **Paramètres Marketing** est affectée aux contacts nouvellement créés.

> [!TIP]  
>   Vous pouvez également créer un client, un fournisseur ou un compte bancaire à partir d'un contact. Pour plus d'informations, reportez-vous à [Créer un client, un fournisseur ou un compte bancaire à partir d'un contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).

## <a name="see-also"></a>Voir aussi
[Synchronisation des contacts avec les clients, les fournisseurs et les comptes bancaires](marketing-synchronize-contacts-customers-vendors-bank-accounts.md)  
[Affecter des relations d'affaires à un contact](marketing-business-relations.md#AssignBusRelContact)  
[Affecter des secteurs d'activité à un contact](marketing-industry-groups.md#AssignIndustryGroupContact)  
[Affecter des groupes de distribution à un contact](marketing-mailing-groups.md#AssignMailGroupContact)  
[Procédure : créer des personnes contact](marketing-create-contact-persons.md)  
[Utilisation de Dynamics NAV](ui-work-product.md)

