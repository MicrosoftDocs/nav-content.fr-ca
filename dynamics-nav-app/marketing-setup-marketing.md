---
title: Informations sur la configuration de la gestion du marketing et des contacts
description: "Vous pouvez configurer la gestion du marketing et des contacts dans Dynamics NAV pour optimiser les relations avec les prospects ou les clients, et améliorer les promotions."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect, client, customer, campaign, promo
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9ff95940c7418bf7cc1265eb128e0c9ccf4fb6c4
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-relationship-management"></a>Paramétrage de la Gestion des relations
Avant de commencer à travailler avec vos contacts et prospects marketing, vous devez prendre certaines décisions et accomplir certaines étapes afin de configurer la façon dont le module marketing gère certains aspects de vos contacts. Par exemple, vous pouvez décider de synchroniser la fiche contact avec la fiche client, la fiche fournisseur, ou la fiche compte bancaire, spécifier comment les séries de numéros sont définies, ou quelles sont les salutations standard lorsque vous écrivez à vos contacts.

La gestion de vos contacts et la mise en place d'une stratégie visant à identifier, attirer et fidéliser les clients permet d'optimiser votre activité et d'accroître la satisfaction des clients. L'utilisation d'un système de gestion de contacts performant permet également de créer et de maintenir les relations avec vos clients. La communication est la clé de ces relations. Pour assurer la réussite de votre entreprise, il est nécessaire de personnaliser la communication avec les clients, fournisseurs et partenaires commerciaux potentiels et existants en fonction de leurs besoins spécifiques. La première étape consiste à établir une stratégie et à définir la manière dont votre compagnie utilise les informations de contact. Dans la mesure où celles-ci seront consultées par de nombreux groupes différents de votre compagnie, la mise en place d'un système performant permettra d'accroître la productivité.

Vous configurez la gestion du marketing et des contacts à partir de la fenêtre **Paramètres marketing**. Pour ouvrir la fenêtre **Paramètres marketing**, choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Paramètres marketing**, puis le lien connexe.

## <a name="automatically-copying-specific-information-from-the-contact-companies-to-the-contact-persons"></a>Copie automatique des informations spécifiques des compagnies contact vers les personnes contact
Une partie des données relatives aux compagnies contact sont identiques aux données sur les personnes contact qui travaillent dans ces compagnies, comme l'adresse. Dans la section **Héritage** de la fenêtre **Paramètres marketing**, vous pouvez définir l'application de sorte qu'elle copier automatiquement des champs spécifiques de la fiche société contact vers la fiche personne contact chaque fois que vous créez une personne contact pour une société contact. Par exemple, vous pouvez choisir de copier un code représentant, les infos adresse (adresse, adresse 2e ligne, ville, code postal et comté), les détails de communication (numéro de télécopieur, numéro de télex et numéro de téléphone), et plus encore.

Lorsque vous modifiez l'un des champs dans la fiche compagnie contact, le programme modifie automatiquement ce champ dans la fiche personne contact (sauf si vous avez modifié ce champ manuellement).

Pour plus d'informations, reportez-vous à [Procédure : créer des personnes contact](marketing-how-create-contact-persons.md).

## <a name="using-predefined-defaults-on-new-contacts"></a>Utilisation de paramètres par défaut prédéfinis sur les nouveaux contacts
Vous pouvez configurer l'application pour qu'elle affecte automatiquement des codes langue, secteur, représentant et pays/région par défaut à chaque nouveau contact. Vous pouvez également entrer un code cycle de vente par défaut que le programme affecte automatiquement à chaque nouvelle opportunité.

Les valeurs héritées des champs sont prioritaires sur les valeurs par défaut que vous avez définies. Par exemple, si vous avez choisi le français comme langue par défaut alors que la langue de la compagnie contact est l'allemand, le programme affecte automatiquement le code langue de l'allemand aux personnes contact enregistrées pour cette compagnie.

<!--You can also setup a default salutation that the program automatically assigns to your contacts. You can use these salutations in your interaction template attachments (for example, Microsoft Word documents). When setting up a default salutation, you can enter a salutation text and a salutation format. For example, if the salutation text is Dear, and the salutation format is Salutation Text + Title + Name, the program will automatically enter Dear Mr. John Smith as a salutation for a contact called John Smith.-->

## <a name="automatically-recording-interactions"></a>Enregistrement automatique des interactions
[!INCLUDE[d365fin](includes/d365fin_md.md)] peut enregistrer automatiquement les documents achat et vente en tant qu'interactions (par exemple, commandes, factures, bons de réception, etc.) ou en tant qu'e-mails, appels téléphoniques et bordereaux d'envoi.

Pour plus d'informations, reportez-vous à [Enregistrer automatiquement les interactions avec les contacts](marketing-auto-record-interactions.md).

## <a name="synchronizing-contacts-with-customers-and-more"></a>Synchronisation des contacts avec les clients et autres
Pour synchroniser la fiche contact avec la fiche client, la fiche fournisseur et la fiche compte bancaire, vous devez sélectionner un code relation d'affaires pour les clients, les fournisseurs et les comptes bancaires. Par exemple, vous ne pouvez lier un contact avec un client existant que si vous avez sélectionné un code relation d'affaires pour les clients dans la fenêtre **Paramètres marketing**.

Pour plus d'informations, reportez-vous à [Procédure de synchronisation des contacts avec les clients, les fournisseurs et les comptes bancaires](marketing-synchronize-contacts-customers-vendors-bank-accounts.md).

## <a name="assigning-a-number-series-to-contacts-and-opportunities"></a>Affectation d'une série de numéros aux contacts et aux opportunités
Vous pouvez configurer des séries de numéros pour les contacts et les opportunités. Si vous avez configuré une série de numéros pour les contacts, lorsque vous créez un contact et que vous appuyez ensuite sur Entrée dans le champ N° de la fiche contact, le programme saisit automatiquement le numéro de contact suivant.

Pour plus d'informations sur les séries de numéros, voir [Procédure : créer des séries de numéros](ui-create-number-series.md).

## <a name="searching-for-duplicate-contacts-when-contacts-are-created"></a>Recherche des doublons lors de la création de contacts
Vous pouvez configurer le programme pour qu'il recherche automatiquement les doublons chaque fois que vous créez une compagnie contact ou vous pouvez choisir d'effectuer une recherche manuelle lorsque les contacts sont créés. Vous pouvez également configurer le programme pour qu'il mette automatiquement à jour les chaînes de recherche chaque fois que vous modifiez les données de contact ou que vous créez un contact. Vous pouvez choisir le pourcentage de chaînes communes, c'est-à-dire le pourcentage de chaînes qui doivent être identiques dans deux contacts pour que le système les considère comme des doublons.

## <a name="see-also"></a>Voir aussi
[Gestion de contacts](marketing-contacts.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

