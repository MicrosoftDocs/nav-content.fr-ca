---
title: "Procédure : réceptionner des articles"
description: "Lorsque les articles arrivent dans un entrepôt configuré pour appeler un traitement de réception entrepôt, vous devez extraire les lignes du document origine libéré ayant déclenché leur réception."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/31/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: d048c52b320a0fcd3cb2f5753c77c3996cd97517
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-receive-items"></a>Procédure : réceptionner des articles
Lorsque les articles arrivent dans un entrepôt qui n'est pas configuré pour un traitement de réception entrepôt, enregistrez simplement la réception du document d'entreprise associé, comme un bon de commande, un retour vente ou un ordre de transfert entrant.

Lorsque les articles arrivent dans un entrepôt configuré pour appeler un traitement de réception entrepôt, vous devez extraire les lignes du document origine libéré ayant déclenché leur réception. En présence de zones, vous pouvez soit accepter la zone par défaut qui est renseignée, soit renseigner la zone de rangement de l'article concerné si cet article n'a jamais été utilisé dans l'entrepôt. Vous devez ensuite renseigner les quantités d'articles reçus et reporter la réception.  

## <a name="to-receive-items-with-a-purchase-order"></a>Pour recevoir des articles avec un bon de commande
La section suivante décrit comment recevoir des articles avec un bon de commande. Les étapes sont similaires pour les retours vente et les ordres de transfert.  
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Bons de commande**, puis sélectionnez le lien associé.
2. Ouvrez un bon de commande existant, ou créez-en un nouveau. Pour plus d'informations, reportez-vous à [Procédure : enregistrer des achats](purchasing-how-record-purchases.md).
3. Dans le champ **Qté à recevoir**, indiquez la quantité reçue.

    La valeur du champ **Qté reçue** est mise à jour en conséquence. Si c'est une réception partielle, la valeur est inférieure à la valeur dans le champ **Quantité**.
4. Sélectionnez l'action **Valider**.

## <a name="to-receive-items-with-a-warehouse-receipt"></a>Pour recevoir des articles avec une réception entrepôt
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Réceptions entrepôt**, puis sélectionnez le lien associé.  
2.  Sélectionnez l'action **Nouveau**.  

    Renseignez les champs du raccourci **Général**. Lorsque vous récupérez des lignes document origine,certaines des informations de l'en-tête sont copiées dans chaque ligne.  

    Pour une configuration entrepôt avec un prélèvement et un rangement suggérés : Si l'emplacement possède des zones par défaut pour les réceptions, les champs **Code de zone** et **Code de zone** seront renseignés automatiquement, mais vous pouvez les modifier selon vos besoins.  

    > [!NOTE]  
    >  Pour recevoir des articles portant des codes classe entrepôt différents du code classe de l'emplacement indiqué dans le champ **Code emplacement** de l'en-tête du document, vous devez supprimer la valeur du champ **Code emplacement** de l'en-tête avant d'extraire les lignes des documents origine des articles.  
3.  Choisissez l'action **Extraire documents origine**. La fenêtre **Documents origine** s'ouvre.

    À partir d'une réception entrepôt nouvelle ou ouverte, vous pouvez utiliser la fenêtre **Filtres pour extr. doc. source** afin d'extraire les lignes du document source libéré qui définissent les articles à recevoir ou à livrer.

    1. Choisissez l'action **Filtrer pour extr. doc. orig.**.  
    2. Pour configurer un nouveau filtre, entrez un code descriptif dans le champ **Code**, puis choisissez l'action **Modifier**.  
    3. Définissez le type de ligne document origine que vous souhaitez extraire en renseignant les champs de filtre appropriés.  
    4. Sélectionnez l'action **Exécuter**.  

    Toutes les lignes du document source libéré qui correspondent aux critères du filtre sont à présent insérées dans la fenêtre **Réception entrepôt** à partir de laquelle vous avez activé la fonction filtre.  

    Les combinaisons de filtres que vous définissez sont stockées dans la fenêtre **Filtres pour extr. doc. orig.** jusqu'à la prochaine utilisation. Le nombre de combinaisons de filtres est illimité. Vous pouvez modifier les critères à tout moment en choisissant l'action **Modifier**.

4.  Sélectionnez le document origine pour lequel vous souhaitez réceptionner des articles, puis sélectionnez le bouton **OK**.  

    Les lignes des documents origine s'affichent dans la fenêtre **Réception entrepôt**. Le champ **Qté à recevoir** est renseigné avec la quantité restante pour chaque ligne, mais vous pouvez modifier cette quantité selon vos besoins. Si vous avez supprimé la valeur du champ **Code emplacement** du raccourci **Général** avant d'accéder aux lignes, vous devez alors renseigner un code emplacement approprié sur chaque ligne réception.  

    > [!NOTE]  
    >  Pour renseigner le champ **Qté à recevoir** sur toutes les lignes à zéro, choisissez l'action **Supprimer qté à recevoir**. Pour y insérer à nouveau la quantité restante, choisissez l'action **Remplir qté à recevoir**.  

    > [!NOTE]  
    >  Vous ne pouvez pas recevoir un nombre d'articles supérieur au nombre figurant dans le champ **Qté ouverte** de la ligne document origine. Pour recevoir des articles supplémentaires, récupérez un autre document origine contenant une ligne pour l'article concerné en utilisant la fonction filtre afin d'obtenir les documents origine où figure cet article.  

5.  Reportez la réception entrepôt. Les champs relatifs à la quantité dans les documents origine sont mis à jour et les articles enregistrés dans le cadre de l'inventaire de la compagnie.  

En cas d'utilisation d'un rangement entrepôt, les lignes réception sont transmises à la fonction de rangement entrepôt. Les articles, bien que réceptionnés, ne peuvent pas être prélevés avant d'avoir été rangés. Les articles réceptionnés sont identifiés en tant qu'inventaire disponible une fois le rangement enregistré uniquement.  

En cas de non-utilisation d'un rangement entrepôt et d'utilisation de zones, le rangement des articles est enregistré dans la zone spécifiée sur la ligne document source.  

> [!NOTE]  
>  En utilisant la fonction **Reporter et Imprimer**, vous effectuez à la fois le report de la réception et l'impression d'une instruction de rangement qui indique où ranger les articles dans le stock.  
>   
>  En cas d'utilisation d'un prélèvement et d'un rangement suggérés, les modèles rangement sont utilisés pour procéder au calcul du meilleur emplacement de rangement des articles. Il est ensuite imprimé sur l'instruction de rangement.  

## <a name="see-also"></a>Voir aussi  
[Gestion d'entrepôt](warehouse-manage-warehouse.md)  
[Stock](inventory-manage-inventory.md)  
[Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md)     
[Gestion d'assemblage](assembly-assemble-items.md)    
[Détails de conception : gestion d'entrepôt](design-details-warehouse-management.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

