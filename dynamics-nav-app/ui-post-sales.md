---
title: Report des ventes
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
ms.openlocfilehash: 0ce8b5d9e77d40a5f10c9242e7368add5b75b12a
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

# <a name="posting-sales"></a>Report des ventes
Dans le groupe **Validation** sur un document vente, vous pouvez faire votre choix parmi les fonctions de validation suivantes :

- **Valider**
- **Impression test**
- **Valider et envoyer**
- **Valider et Imprimer**
- **Valider et envoyer par e-mail**
- **Valider par lot**
- **Aperçu compta.**

Lorsque vous avez renseigné toutes les lignes et entré toutes les informations du document de vente, vous pouvez le reporter. Cela crée une livraison et une facture.

Lorsqu’un document de vente est reporté, le compte du client, le grand livre et les écritures article sont mis à jour.

Pour chaque commande vente, une écriture vente est créée dans la table **Écriture comptable**. Une écriture est également créée dans le compte client de la table **Écriture comptable client** et une écriture comptable est créée dans le compte client approprié. De plus, le report de la commande peut avoir pour résultat la création d’une écriture TVA et d’une écriture GL pour le montant de l'escompte. La validation d’une écriture pour la remise dépend de la valeur du champ **Comptabilisation remises** de la fenêtre **Paramètres ventes**.

Pour chaque ligne commande vente, une écriture comptable article est créée dans la table **Écriture comptable article** (si les lignes vente contiennent des numéros des articles) ou une écriture comptable est créée dans la table **Écriture comptable** (si les lignes vente contiennent un compte général). En outre, les commandes vente sont toujours enregistrées dans les tables **En-tête expédition vente** et **En-tête facture vente**.

**Important** : lorsque vous validez une commande, vous pouvez créer à la fois une expédition et une facture. Ceci peut être effectué de manière simultanée ou indépendante. Vous pouvez également créer une expédition partielle et une facture partielle en renseignant les champs **Qté à expédier** et **Qté à facturer** sur chaque ligne commande vente avant la validation. Notez que vous ne pouvez pas créer de facture pour un article qui n'est pas livré. C'est-à-dire que, avant de pouvoir facturer, vous devez avoir reporté une livraison, ou vous devez choisir de livrer et de facturer en même temps. 

Lorsque le report est terminé, les lignes vente reportées sont supprimées de la commande. Un message vous indique lorsque le report est terminé. Vous pouvez ensuite afficher les écritures validées dans les diverses fenêtres qui contiennent les écritures validées, telles que **Écritures comptables client**, **Écritures comptables**, **Écritures comptables article**, **Expéditions vente enregistrées** et **Factures vente enregistrées**.

## <a name="see-also"></a>Voir aussi
[Procédure : envoyer des documents par e-mail](ui-how-send-documents-email.md)

