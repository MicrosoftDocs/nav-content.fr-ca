---
title: Report des achats
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c03d031e951bc185b18bedaf428d414c1fe2e7d1
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="posting-purchases"></a>Report des achats
Dans le groupe **Validation** sur un document achat, vous pouvez faire votre choix parmi les fonctions de validation suivantes :

- **Valider**
- **Aperçu compta.**
- **Valider et Imprimer**
- **Impression test**
- **Valider par lot**

Lorsque vous avez renseigné toutes les lignes et saisi toutes les informations du bon de commande, vous pouvez le reporter, c'est-à-dire, créer une réception et une facture.

Lorsqu’un bon de commande est reporté, le compte du fournisseur, le grand livre et les écritures article sont mis à jour.

Pour chaque commande achat, une écriture achat est créée dans la table **Ecriture comptable**. Une écriture est également créée dans le compte fournisseur de la table **Ecriture fournisseur** et une autre dans le compte fournisseur approprié. De plus, le report de la commande peut avoir pour résultat la création d'une écriture TVA et d'une écriture pour le montant de l'escompte. La validation d'une écriture pour la remise dépend de la valeur du champ **Comptabilisation remise** de la fenêtre **Paramètres achats**.

Pour chaque ligne commande achat, une écriture comptable article est créée dans la table **Écriture comptable article** (si les lignes achat contiennent des numéros d'article) ou une écriture est créée dans la table **Écriture comptable** (si les lignes achat contiennent un compte général). En outre, les commandes achat sont toujours enregistrées dans les tables **En-tête réception achat** et **En-tête facture achat**.

Avant de commencer à reporter, vous pouvez effectuer une rapport de test qui contient toutes les informations du bon de commande et indique les erreurs afférentes. Pour imprimer l’état, sélectionnez **Validation**, puis **Impression test**.

**Important**: lorsque vous validez une commande, vous pouvez créer à la fois une réception et une facture. Celles-ci peuvent être faites simultanément ou séparément. Vous pouvez également créer une réception partielle et une facture partielle en renseignant les champs **Qté à recevoir** et **Qté à facturer** sur chaque ligne commande achat avant la validation. Remarquez que vous ne pouvez pas créer de facture pour un article qui n'a pas été reçu. C'est-à-dire que, avant de pouvoir facturer, vous devez avoir validé une réception, ou vous devez choisir de réceptionner et de facturer en même temps.

Vous pouvez soit reporter, soit reporter et imprimer. Si vous choisissez de reporter et d’imprimer, un rapport est imprimé lorsque la commande est reportée. Vous pouvez aussi choisir la fonction **Valider par lot**, qui vous permet de valider plusieurs commandes en même temps.

Lorsque le report est terminé, les lignes achat reportées sont supprimées de la commande. Un message vous indique lorsque le report est terminé. Vous pouvez ensuite afficher les écritures validées dans les diverses fenêtres qui contiennent les écritures validées, comme les fenêtres **Écritures comptable fournisseur**, **Écritures comptable**, **Écritures comptable article**, **Réceptions achat enreg.** et **Factures achat enregistrées**.

## <a name="see-also"></a>Voir aussi
[Valider des documents et des feuilles](ui-post-documents-journals.md)

