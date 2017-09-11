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
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: e87dd5faf7713aecfbe7209d00bb8076fcae9d25
ms.contentlocale: fr-ca
ms.lasthandoff: 07/19/2017

---

# <a name="posting-sales"></a><span data-ttu-id="f1d0a-102">Report des ventes</span><span class="sxs-lookup"><span data-stu-id="f1d0a-102">Posting Sales</span></span>
<span data-ttu-id="f1d0a-103">Dans le groupe **Validation** sur un document vente, vous pouvez faire votre choix parmi les fonctions de validation suivantes :</span><span class="sxs-lookup"><span data-stu-id="f1d0a-103">In the **Posting group** on a sales document, you can choose between the following posting functions:</span></span>

- <span data-ttu-id="f1d0a-104">**Valider**</span><span class="sxs-lookup"><span data-stu-id="f1d0a-104">**Post**</span></span>
- <span data-ttu-id="f1d0a-105">**Impression test**</span><span class="sxs-lookup"><span data-stu-id="f1d0a-105">**Test Report**</span></span>
- <span data-ttu-id="f1d0a-106">**Valider et envoyer**</span><span class="sxs-lookup"><span data-stu-id="f1d0a-106">**Post and Send**</span></span>
- <span data-ttu-id="f1d0a-107">**Valider et Imprimer**</span><span class="sxs-lookup"><span data-stu-id="f1d0a-107">**Post and Print**</span></span>
- <span data-ttu-id="f1d0a-108">**Valider et envoyer par e-mail**</span><span class="sxs-lookup"><span data-stu-id="f1d0a-108">**Post and Email**</span></span>
- <span data-ttu-id="f1d0a-109">**Valider par lot**</span><span class="sxs-lookup"><span data-stu-id="f1d0a-109">**Post Batch**</span></span>
- <span data-ttu-id="f1d0a-110">**Aperçu compta.**</span><span class="sxs-lookup"><span data-stu-id="f1d0a-110">**Preview Posting**</span></span>

<span data-ttu-id="f1d0a-111">Lorsque vous avez renseigné toutes les lignes et entré toutes les informations du document de vente, vous pouvez le reporter.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-111">When you have completed all the lines and entered all the information on the sales order, you can post it.</span></span> <span data-ttu-id="f1d0a-112">Cela crée une livraison et une facture.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-112">This creates a shipment and an invoice.</span></span>

<span data-ttu-id="f1d0a-113">Lorsqu’un document de vente est reporté, le compte du client, le grand livre et les écritures article sont mis à jour.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-113">When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.</span></span>

<span data-ttu-id="f1d0a-114">Pour chaque commande vente, une écriture vente est créée dans la table **Écriture comptable**.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-114">For each sales order, a sales entry is created in the **G/L Entry** table.</span></span> <span data-ttu-id="f1d0a-115">Une écriture est également créée dans le compte client de la table **Écriture comptable client** et une écriture comptable est créée dans le compte client approprié.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-115">An entry is also created in the customer's account in the **Cust. Ledger Entry** table and a general ledger entry is created in the relevant receivables account.</span></span> <span data-ttu-id="f1d0a-116">De plus, le report de la commande peut avoir pour résultat la création d’une écriture TVA et d’une écriture GL pour le montant de l'escompte.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-116">In addition, posting the order may result in a VAT entry and a general ledger entry for the discount amount.</span></span> <span data-ttu-id="f1d0a-117">La validation d’une écriture pour la remise dépend de la valeur du champ **Comptabilisation remises** de la fenêtre **Paramètres ventes**.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-117">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field in the **Sales & Receivables Setup** window.</span></span>

<span data-ttu-id="f1d0a-118">Pour chaque ligne commande vente, une écriture comptable article est créée dans la table **Écriture comptable article** (si les lignes vente contiennent des numéros des articles) ou une écriture comptable est créée dans la table **Écriture comptable** (si les lignes vente contiennent un compte général).</span><span class="sxs-lookup"><span data-stu-id="f1d0a-118">For each sales order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the sales lines contain item numbers) or a general ledger entry will be created in the **G/L Entry** table (if the sales lines contain a general ledger account).</span></span> <span data-ttu-id="f1d0a-119">En outre, les commandes vente sont toujours enregistrées dans les tables **En-tête expédition vente** et **En-tête facture vente**.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-119">In addition to this, sales orders are always recorded in the **Sales Shipment Header** and **Sales Invoice Header** tables.</span></span>

<span data-ttu-id="f1d0a-120">**Important** : lorsque vous validez une commande, vous pouvez créer à la fois une expédition et une facture.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-120">**Important**: When you post an order, you can create both a shipment and an invoice.</span></span> <span data-ttu-id="f1d0a-121">Ceci peut être effectué de manière simultanée ou indépendante.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-121">These can be done at the same time or independently.</span></span> <span data-ttu-id="f1d0a-122">Vous pouvez également créer une expédition partielle et une facture partielle en renseignant les champs **Qté à expédier** et **Qté à facturer** sur chaque ligne commande vente avant la validation.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-122">You can also create a partial shipment and a partial invoice by completing the **Qty. to Ship** and **Qty. to Invoice** fields on the individual sales order lines before you post.</span></span> <span data-ttu-id="f1d0a-123">Notez que vous ne pouvez pas créer de facture pour un article qui n'est pas livré.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-123">Note that you cannot create an invoice for something that is not shipped.</span></span> <span data-ttu-id="f1d0a-124">C'est-à-dire que, avant de pouvoir facturer, vous devez avoir reporté une livraison, ou vous devez choisir de livrer et de facturer en même temps.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-124">That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.</span></span> 

<span data-ttu-id="f1d0a-125">Lorsque le report est terminé, les lignes vente reportées sont supprimées de la commande.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-125">When the posting is completed, the posted sales lines are removed from the order.</span></span> <span data-ttu-id="f1d0a-126">Un message vous indique lorsque le report est terminé.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-126">A message tells you when the posting is completed.</span></span> <span data-ttu-id="f1d0a-127">Vous pouvez ensuite afficher les écritures validées dans les diverses fenêtres qui contiennent les écritures validées, telles que **Écritures comptables client**, **Écritures comptables**, **Écritures comptables article**, **Expéditions vente enregistrées** et **Factures vente enregistrées**.</span><span class="sxs-lookup"><span data-stu-id="f1d0a-127">After this, you will be able to see the posted entries in the various windows that contain posted entries, such as the **Cust. Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Posted Sales Shipments**, and **Posted Sales Invoices** windows.</span></span>

## <a name="see-also"></a><span data-ttu-id="f1d0a-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1d0a-128">See Also</span></span>
[<span data-ttu-id="f1d0a-129">Procédure : envoyer des documents par e-mail</span><span class="sxs-lookup"><span data-stu-id="f1d0a-129">How to: Send Documents by Email</span></span>](ui-how-send-documents-email.md)

