---
title: "Créer une fiche fournisseur pour enregistrer un nouveau fournisseur"
description: "Apprendre comment créer une fiche fournisseur pour enregistrer un nouveau fournisseur."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c7fee8b43940fc5e5fb020b4ca1ac9b27b90decd
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-register-new-vendors"></a>Procédure : enregistrer de nouveaux fournisseurs
Les fournisseurs fournissent les produits que vous vendez. Chaque fournisseur à qui vous achetez des biens doit être enregistré en tant que fiche fournisseur.

Avant de pouvoir enregistrer de nouveaux fournisseurs, vous devez configurer divers codes achat que vous pouvez sélectionner lorsque vous renseignez les fiches fournisseur. Lorsque toutes les données de base requises sont créées, vous pouvez configurer des éléments supplémentaires sur le fournisseur, comme par exemple attribuer une priorité au fournisseur à des fins de paiement et répertorier les articles que les fournisseurs peuvent fournir. Un autre groupe de tâches de configuration consiste à enregistrer vos accords concernant les remises, les prix et les modes de règlement. Pour plus d'informations, reportez-vous à [Définition des achats](purchasing-setup-purchasing.md).

Les fiches fournisseur contiennent les informations requises pour acheter des produits au fournisseur. Pour plus d'informations, reportez-vous à [Procédure : enregistrer des achats](purchasing-how-record-purchases.md) et à [Procédure : enregistrer de nouveaux articles](inventory-how-register-new-items.md).

> [!NOTE]  
>   Si des modèles fournisseur existent pour différents types de fournisseurs, une fenêtre s'affiche lorsque vous créez une fiche fournisseur à partir de laquelle vous pouvez sélectionner un modèle approprié. Si un seul modèle fournisseur existe, les nouvelles fiches fournisseur utiliseront toujours ce modèle.

## <a name="to-create-a-new-vendor-card"></a>Pour créer une fiche fournisseur
1. Sur la page d'accueil, sélectionnez **Fournisseurs** pour ouvrir la liste des fournisseur existants.  
2. Dans la fenêtre **Fournisseurs**, sélectionnez l'action **Nouveau**.

    Si plusieurs modèles de fournisseur existent, une fenêtre s'affiche et vous permet de sélectionner un modèle fournisseur. Dans ce cas, suivez les deux étapes suivantes.
3. Dans la fenêtre **Sélectionnez un modèle pour un nouveau fournisseur**, sélectionnez le modèle que vous souhaitez utiliser pour la nouvelle fiche fournisseur.
4. Cliquez sur le bouton **OK**. Une nouvelle fiche fournisseur avec certains champs contenant les informations provenant de ce modèle s'ouvre.
5. Renseignez ou modifiez les champs de la fiche fournisseur selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   Si vous ne savez pas l'adresse de facturation qui sera utilisée pour chaque facture d'un fournisseur, ne renseignez pas le champ **Paiement**. Sélectionnez plutôt le numéro du fournisseur créancier après avoir configuré un devis, une commande ou un en-tête facture.

Le fournisseur est désormais enregistré, et la fiche fournisseur est prête à être utilisée sur les documents d'achat.

Si vous souhaitez utiliser cette fiche fournisseur comme modèle lorsque vous créez de nouvelles fiches fournisseur, enregistrez-la comme modèle fournisseur. Pour plus d'informations, reportez-vous à la section suivantes.

## <a name="to-save-the-vendor-card-as-a-template"></a>Pour enregistrer la fiche fournisseur en tant que modèle
1. Dans la fenêtre **Fiche fournisseur**, sélectionnez l'action **Sauvegarder comme modèle**. La fenêtre **Modèle fournisseur** s'ouvre et affiche la fiche fournisseur comme modèle.
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Pour réutiliser les axes analytiques dans les modèles, sélectionnez l'action **Axes analytiques**. La fenêtre **Modèles axe** s'ouvre et affiche tous les codes axe qui sont définis pour le fournisseur.
4. Modifiez ou entrez les codes dimension s'appliquant aux nouvelles fiches fournisseur créées à l'aide du modèle.
5. Lorsque vous avez terminé le nouveau modèle fournisseur, cliquez sur le bouton **OK**.  
   Le modèle fournisseur est ajouté à la liste des modèles fournisseur. Vous pouvez ainsi l'utiliser pour créer des fiches fournisseur.

## <a name="see-also"></a>Voir aussi
[Achats](purchasing-manage-purchasing.md)  
[Procédure : enregistrer des achats](purchasing-how-record-purchases.md)   
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

