---
title: Inventaire, ajustement et reclassement de l'inventaire
description: "Décrit la manière d'effectuer un inventaire physique, faire des ajustements négatifs ou positifs, et comment modifier des informations, telles que l'emplacement ou le numéro de lot, sur des écritures article ou des écritures entrepôt."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: adjustment, negative, positive, increase, decrease
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 4d53e6e9b64e0f5c790abb0f62f66a2b28c12c50
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-count-adjust-and-reclassify-inventory"></a>Procédure : Inventaire, ajustement et reclassement de l'inventaire
Vous devez effectuer un inventaire (c'est-à-dire compter tous les articles disponibles) au moins une fois par exercice pour vérifier si la quantité enregistrée dans la base de données est identique à la quantité réelle en stock dans les entrepôts. Lorsque vous connaissez la quantité physique réelle, vous devez la reporter dans le grand livre dans le cadre de l'évaluation de l'inventaire de fin d'exercice.

Bien que vous comptiez tous les articles de l'inventaire au moins une fois par an, vous pouvez avoir décidé de compter certains articles plus souvent, parce qu'ils ont plus de valeur ou parce qu'ils sont très demandés et représentent une partie importante de votre activité. Pour cela, vous pouvez affecter des périodes d'inventaire spéciales à ces articles. Pour plus d'informations, reportez-vous à la section « Effectuer un inventaire tournant ».

Pour ajuster les quantités d'inventaire enregistrées, pour inventaire ou à d'autres fins, vous pouvez utiliser un journal article pour modifier les écritures du grand livre de l'inventaire directement sans reporter les transactions commerciales. Sinon, vous pouvez ajuster pour un article distinct de la fiche article.

Pour modifier les attributs du grand livre article et les quantités, vous pouvez utiliser le journal reclassement article. Les attributs courants pour les reclassements incluent les numéros de série et/ou de lot, les dates d'expiration et les dimensions.

> [!NOTE]
> Dans les configurations d'entrepôt avancées, les articles sont enregistrés dans des zones en tant qu'écritures entrepôt, pas en tant qu'écritures article. Par conséquent, vous effectuez l'inventaire, l'ajustement et le reclassement dans des journaux d'entrepôt spéciaux qui prennent en charge les zones. Ensuite, vous utilisez des fonctions spéciales pour synchroniser les écritures entrepôt nouvelles ou modifiées avec leurs écritures article correspondantes pour refléter les modifications des quantités et valeurs d'inventaire. Ceci est décrit dans des procédures spécifiques ci-dessous lorsque cela est approprié.

## <a name="to-perform-a-physical-inventory"></a>Pour effectuer un inventaire physique
À la fin de l'exercice financier, ou plus souvent, vous devez effectuer un inventaire, c'est-à-dire compter les articles réellement disponibles, pour vérifier si la quantité enregistrée correspond à la quantité réelle de l'inventaire. S'il existe des différences, vous devez les reporter dans les comptes article avant de procéder à l'évaluation de l'inventaire.

Outre la tâche de comptage réelle, le processus complet implique les trois tâches suivantes :

- Calculez l'inventaire prévu.
- Imprimer le rapport à utiliser lors du comptage.
- Entrez et reportez l'inventaire calculé réel.

Vous pouvez effectuer l'inventaire physique de l'une des manières suivantes en fonction de votre configuration entrepôt. Pour plus d'informations, voir [Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md).  

-   Si votre emplacement n'utilise pas le prélèvement et rangement suggérés (configuration d'entrepôt de base), vous pouvez utiliser la fenêtre **Journal inventaire physique** du menu **Inventaire** ; la procédure est similaire à celle d'un inventaire physique sans inventaire périodique.  
-   Si votre emplacement utilise le prélèvement et rangement suggérés (configuration d'entrepôt avancée), vous utilisez d'abord la fenêtre **Journal inventaire physique entrepôt**, puis la fenêtre **Journal article** pour exécuter la fonction **Calculer ajustement entrepôt**.

### <a name="to-calculate-the-expected-inventory-in-basic-warehouse-configurations"></a>Pour calculer l'inventaire prévu dans les configurations d'entrepôt de base
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles inventaire**, puis sélectionnez le lien connexe.
2. Choisissez l'action **Calculer stock**.
3. Dans la fenêtre **Calculer stock**, indiquez les conditions à utiliser pour créer les lignes feuille, par exemple si vous souhaitez inclure les articles pour lesquels aucun stock n'est enregistré.
4. Définissez des filtres si vous souhaitez uniquement calculer l'inventaire de certains articles, zones, emplacements ou dimensions.
5. Cliquez sur le bouton **OK**.

> [!NOTE]  
>   Les écritures article sont traitées en fonction des informations que vous avez indiquées, et les lignes sont créées dans le journal inventaire physique. Notez que le champ **Qté (constatée)** est renseigné automatiquement avec la même quantité que le champ **Qté (calculée)**. Avec cette fonction, vous n'avez pas besoin d'entrer l'inventaire disponible pour les articles dont le nombre correspond à la quantité calculée. Toutefois, si la quantité comptée diffère de ce qui est saisi dans le champ **Qté (calculée)**, vous devez la remplacer par la quantité réellement comptée.

### <a name="to-calculate-the-expected-inventory-in-advanced-warehouse-configurations"></a>Pour calculer l'inventaire prévu dans les configurations d'entrepôt avancées
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Journal article**, et sélectionnez le lien associé.  
2.  Sélectionnez l'action **Calculer ajustement entrepôt**.  
3.  Renseignez le formulaire de sélection du traitement en lot en y indiquant votre emplacement et les numéros des articles que vous souhaitez compter.
4. Cliquez sur le bouton **OK**, puis validez les éventuels ajustements.

    Si vous n'effectuez pas cette opération avant d'exécuter l'inventaire entrepôt, les résultats que vous reportez dans le journal inventaire physique et le grand livre d'inventaire physique dans la deuxième partie de la procédure seront les résultats de l'inventaire physique combinés avec d'autres ajustements entrepôt pour les articles comptés.  
5.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Journal inventaire physique entrepôt**, puis sélectionnez le lien associé.  
6. Choisissez l'action **Calculer stock**. Le formulaire de sélection du traitement par lots **Calculer stock entrepôt** s'ouvre.  
7.  Positionnez les filtres permettant de limiter les articles comptés dans la feuille, puis sélectionnez le bouton **OK**.

    Le programme crée une ligne pour chaque zone répondant aux exigences des filtres. À ce stade, vous pouvez encore supprimer certaines lignes, mais si vous souhaitez reporter les résultats en tant qu'inventaire physique, vous devez compter l'article dans toutes les zones le contenant.  

     Si le temps dont vous disposez vous permet uniquement de compter l'article dans certains emplacements, vous pouvez noter les différences, les enregistrer, puis les valider dans la feuille article à l'aide de la fonction **Calculer ajustement entrepôt**.  
8.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Liste de l'inventaire physique de l'entrepôt**, puis sélectionnez le lien associé.  
9.  Ouvrez la page de sélection du rapport, puis imprimez les listes sur lesquelles vous souhaitez que les employés enregistrent la quantité d'articles qu'ils comptent dans chaque zone.  
10. Une fois le décompte effectué, saisissez les quantités comptées dans le champ **Qté (Inventaire physique)** du journal inventaire physique entrepôt.  

    > [!NOTE]  
    >  Dans le journal inventaire physique entrepôt, le champ **Qté (calculée)** est renseigné automatiquement sur la base des enregistrements de zone de stockage et copie ces quantités sur chaque ligne du champ **Qté (physique)**. Si la quantité comptée par l'employé d'entrepôt est différente de celle renseignée par le programme dans le champ Qté (constatée), vous devez entrer la quantité réellement comptée.  

11. Lorsque vous avez entré toutes les quantités comptées, sélectionnez l'action **Enregistrer**.  

    Lorsque vous enregistrez le journal, le programme crée dans l'historique entrepôt deux écritures entrepôt pour chaque ligne comptée et enregistrée :  

    -   Si les quantités calculées et les quantités réelles sont différentes, une quantité négative ou positive est enregistrée pour la zone, et une quantité équilibrée est reportée dans la zone d'ajustement de l'emplacement.  
    -   Si la quantité calculée est égale à la quantité réelle, le programme enregistre une écriture de 0 pour la zone et la zone d'ajustement. Les écritures indiquent qu'à la date d'enregistrement, un inventaire entrepôt a été effectué et qu'il n'y avait aucune différence pour l'article au niveau de l'inventaire.  

Lorsque vous enregistrez l'inventaire entrepôt, vous ne reportez ni dans le grand livre article, ni dans le grand livre d'inventaire physique, ni dans l'écriture valeur, mais les enregistrements peuvent être utilisés lorsqu'un rapprochement immédiat est nécessaire. Cependant, si vous souhaitez conserver des enregistrements précis des événements entrepôt et que vous avez compté toutes les zones où les articles étaient enregistrés, reportez immédiatement les résultats entrepôt en tant qu'inventaire physique. Pour plus d'informations, voir la section « Pour saisir et reporter l'inventaire réel comptabilisé dans les configurations d'entrepôt avancées ».

### <a name="to-print-the-report-to-be-used-when-counting"></a>Pour imprimer le rapport à utiliser lors du comptage
1. Dans la fenêtre **Feuille inventaire** contenant le stock prévu calculé, choisissez l'action **Imprimer**.
2. Dans la fenêtre **Liste d'inventaire**, indiquez si l'état doit indiquer la quantité calculée et si l'état doit répertorier les articles en stock par numéros de série/lot.
3. Définissez des filtres si vous souhaitez uniquement imprimer le rapport pour certains articles, zones, emplacements ou dimensions.
4. Cliquez sur le bouton **Imprimer**.

Les employés peuvent maintenant poursuivre le comptage de l'inventaire et noter les éventuelles différences sur le rapport imprimé.

### <a name="to-enter-and-post-the-actual-counted-inventory-in-basic-warehouse-configurations"></a>Pour saisir et reporter l'inventaire réel comptabilisé dans les configurations d'entrepôt de base
1. Sur chaque ligne de la fenêtre **Feuilles inventaire** sur laquelle le stock réellement disponible, comme déterminé par le comptage, diffère de la quantité calculée, saisissez la quantité réellement disponible dans le champ **Qté (constatée)**.

    Les champs associés sont mis à jour en conséquence.

    > [!NOTE]  
>   Si l'inventaire physique fait apparaître des différences dues à des articles reportés avec des codes emplacement incorrects, n'indiquez pas les différences dans le journal inventaire physique. Au lieu de cela, utilisez le journal reclassement ou un ordre de transfert pour rediriger les articles vers les emplacements appropriés. Pour plus d'informations, voir Feuille reclassement article ou Procédure : créer des ordres de transfert.

2. Pour ajuster les quantités calculées avec les quantités comptées réelles, choisissez **Valider**.

    Les écritures du grand livre d'articles et les écritures du grand livre de l'inventaire physique sont créées. Ouvrez la fiche article pour visualiser les écritures de grand livre d'inventaire physique ainsi obtenues.

3. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Articles**, puis sélectionnez le lien connexe.
4. Pour vérifier l'inventaire de stock, ouvrez la fiche article en question, puis choisissez **Écritures comptables inventaire**.

### <a name="to-enter-and-post-the-actual-counted-inventory-in-advanced-warehouse-configurations"></a>Pour saisir et reporter l'inventaire réel comptabilisé dans les configurations d'entrepôt avancées

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Journal article**, et sélectionnez le lien associé.  
2.  Sélectionnez l'action **Calculer ajustement entrepôt**.  
3.  Sélectionnez les articles que vous avez compté au cours de l'inventaire que vous venez de réaliser, et tous les autres articles nécessitant un ajustement, puis choisissez le bouton **OK**.  

     La fenêtre **Feuille inventaire** s'ouvre et des lignes sont créées pour ces articles. Remarquez que les quantités nettes que vous venez de compter et d'enregistrer zone par zone sont à présent prêtes à être consolidées et synchronisées comme écritures article.  

4.  Reportez le journal sans modifier les quantités.  

Les quantités du grand livre article (écritures article) et les quantités de l'entrepôt (écritures entrepôt) sont une nouvelle fois identiques pour ces articles ; en outre, le programme a mis à jour la dernière date inventaire de l'article ou de l'unité de stock.  

## <a name="to-perform-cycle-counting"></a>Pour effectuer l'inventaire périodique
Bien que vous comptiez tous les articles de l'inventaire au moins une fois par an, vous pouvez avoir décidé de compter certains articles plus souvent, parce qu'ils ont plus de valeur ou parce qu'ils sont très demandés et représentent une partie importante de votre activité. Pour cela, vous pouvez affecter des périodes d'inventaire spéciales à ces articles.

Vous pouvez effectuer un inventaire tournant de l'une des manières suivantes en fonction de votre configuration entrepôt. Pour plus d'informations, voir [Configuration de la gestion des entrepôts](warehouse-setup-warehouse.md).  

-   Si votre emplacement n'utilise pas le prélèvement et rangement suggérés (configuration d'entrepôt de base), vous pouvez utiliser la fenêtre **Journal inventaire physique** du menu **Inventaire** ; la procédure est similaire à celle d'un inventaire physique sans inventaire périodique.  
-   Si votre emplacement utilise le prélèvement et rangement suggérés (configuration d'entrepôt avancée), vous utilisez d'abord la fenêtre **Journal inventaire physique entrepôt**, puis la fenêtre **Journal article** pour exécuter la fonction **Calculer ajustement entrepôt**.  

### <a name="to-set-up-counting-periods"></a>Pour configurer des périodes d'inventaire
Un inventaire est généralement effectué en fonction d'intervalles récurrents (par exemple, tous les mois, tous les trimestres ou toutes les années). Vous pouvez configurer les périodes d'inventaire nécessaires.

Configurez les périodes d'inventaire que vous souhaitez utiliser, puis affectez-en une à chaque article. Lorsque vous effectuez un inventaire et que vous utilisez **Calculer période d'inventaire** de la feuille inventaire, les lignes des articles sont créées automatiquement.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Périodes inventaire**, puis sélectionnez le lien connexe.  
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

### <a name="to-assign-a-counting-period-to-an-item"></a>Pour affecter une période d'inventaire à un article  
1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Articles**, puis sélectionnez le lien connexe.  
2. Sélectionnez l'article auquel vous souhaitez affecter une période d'inventaire.  
3. Dans le champ **Code période inventaire stock**, sélectionnez la période d'inventaire appropriée.  
4. Cliquez sur le bouton **Oui** pour modifier le code et la calculer la première période d'inventaire de l'article. La prochaine fois que vous choisissez de calculer une période d'inventaire dans la feuille inventaire, l'article s'affichera en tant que ligne dans la fenêtre **Sélection article inventaire**. Vous pouvez ensuite commencer à compter l'article sur une base périodique.

### <a name="to-initiate-a-count-based-on-counting-periods-in-basic-warehouse-configurations"></a>Pour lancer un décompte selon des périodes d'inventaire dans les configurations d'entrepôt de base
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuille inventaire**, puis sélectionnez le lien connexe.
2. Choisissez l'action **Calculer la période d'inventaire**.

    La fenêtre **Sélection article inventaire** qui s'ouvre affiche les articles auxquels des périodes d'inventaire ont été affectés et qui doivent être comptés en fonction de leurs périodes d'inventaire.
3. Effectuer l'inventaire physique. Pour plus d'informations, voir la section « Pour effectuer un inventaire physique ».

### <a name="to-initiate-a-count-based-on-counting-periods-in-advanced-warehouse-configurations"></a>Pour lancer un décompte selon des périodes d'inventaire dans les configurations d'entrepôt avancées
1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Journal inventaire physique entrepôt**, puis sélectionnez le lien associé.  
2. Choisissez l'action **Calculer la période d'inventaire**.

    La fenêtre **Sélection article inventaire** qui s'ouvre affiche les articles auxquels des périodes d'inventaire ont été affectés et qui doivent être comptés en fonction de leurs périodes d'inventaire.
3. Effectuer l'inventaire physique. Pour plus d'informations, voir la section « Pour effectuer un inventaire physique ».  

    > [!NOTE]  
    >  Vous devez compter l'article dans tous les emplacements contenant cet article. Si vous supprimez certaines des lignes emplacement que le programme a récupérées dans la fenêtre **Inventaire entrepôt** , vous ne compterez pas tous les articles dans l'entrepôt. Si vous reportez ultérieurement ces résultats incomplets dans le journal inventaire physique, les montants reportés sont incorrects.  

## <a name="to-adjust-the-inventory-of-one-item"></a>Pour ajuster l'inventaire d'un article
Après avoir effectué un inventaire d'un article dans votre module Distribution - Stocks, vous pouvez utiliser la fonction **Ajuster stock** pour enregistrer la quantité réelle en stock.

1. Choisissez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Articles**, puis sélectionnez le lien connexe.
2. Sélectionnez l'article pour lequel vous souhaitez ajuster le stock, puis sélectionnez l'action **Ajuster stock**.
3. Dans le champ **Nouveau stock**, entrez la quantité en stock que vous souhaitez enregistrer pour l'article.
4. Cliquez sur le bouton **OK**.

L'inventaire de l'article est désormais ajusté. La nouvelle quantité s'affiche dans le champ **Stock actuel** de la fenêtre **Ajuster stock** et dans le champ **Stock** de la fenêtre **Fiche article**.

Vous pouvez également utiliser la fonction **Ajuster stock** comme un moyen simple de placer les articles achetés dans le stock si vous n'utilisez pas des factures achat ou des commandes pour enregistrer vos achats. Pour plus d'informations, reportez-vous à [Procédure : enregistrer des achats](purchasing-how-record-purchases.md).

> [!NOTE]  
>   Après avoir ajusté l'inventaire, vous devez le mettre à jour avec la valeur actuelle calculée. Pour plus d'informations, voir [Procédure : réévaluer le stock](inventory-how-revalue-inventory.md).

### <a name="to-adjust-the-inventory-quantity-of-multiple-items-in-basic-warehouse-configurations"></a>Pour ajuster la quantité en inventaire de plusieurs articles dans les configurations d'entrepôt de base
Dans la fenêtre **feuille article**, vous pouvez valider la transaction article directement pour ajuster le stock en fonction des achats, ventes et d'ajustements positifs et négatifs sans utiliser de documents.

Si vous utilisez fréquemment la feuille article pour comptabiliser des lignes feuille identiques ou analogues (par exemple, des lignes en rapport avec la consommation de matériel), vous pouvez utiliser la fenêtre **Feuille article standard** pour simplifier cette tâche récurrente. Pour plus d'informations, reportez-vous à la section « Feuilles standard » de [Utilisation de feuilles comptabilité](ui-work-general-journals.md).

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles article**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Choisissez l'action **Valider** pour créer des ajustements de stock.

> [!NOTE]  
>   Après avoir ajusté l'inventaire, vous devez le mettre à jour avec la valeur actuelle calculée. Pour plus d'informations, voir [Procédure : réévaluer le stock](inventory-how-revalue-inventory.md).

### <a name="to-adjust-bin-quantities-in-advanced-warehouse-configurations"></a>Pour ajuster les quantités de zone dans les configurations d'entrepôt avancées  
Si votre emplacement utilise des prélèvement et rangement suggérés, vous pouvez utiliser le **journal article entrepôt** pour reporter, hors inventaire physique, tous les ajustements positifs et négatifs au niveau de la quantité article qui sont des gains réels, tels que les articles précédemment reportés comme manquants et qui apparaissent subitement, ou des pertes réelles, telles que les bris d'articles fragiles.  

Contrairement au report des ajustements dans le journal article inventaire, l'utilisation du journal article entrepôt permet d'obtenir un autre niveau d'ajustement des enregistrements de quantité encore plus précis, à tout moment. Par conséquent, l'entrepôt dispose toujours d'un enregistrement complet indiquant le nombre d'articles disponibles et leur lieu de stockage, mais les enregistrements ajustement ne sont pas immédiatement reportés dans le grand livre article. Au cours de l'enregistrement, le programme crédite ou débite la zone de l'ajustement quantité, et crée une écriture de compensation dans la zone d'ajustement entrepôt (zone virtuelle sans articles réels). Cette zone a été définie dans le **Code de zone d'ajustement inventaire** sur la fiche emplacement.

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Journal article entrep.**, puis sélectionnez le lien associé.  
2.  Renseignez les informations d'ent-ête.  
3.  Renseignez le champ **N° article** de la ligne.  
4.  Saisissez la zone dans laquelle vous placez les articles supplémentaires ou dans laquelle des articles sont manquants.  
5.  Saisissez la différence de quantité dans le champ **Quantité**. Si vous avez trouvé des articles supplémentaires, saisissez une quantité positive. Si des articles sont manquants, saisissez une quantité négative.  
6.  Sélectionnez l'action **Enregistrer**.

## <a name="to-synchronize-the-adjusted-warehouse-entries-with-the-related-item-ledger-entries"></a>Pour synchroniser les écritures entrepôt ajustées avec les écritures article associées
Suivant les intervalles définis par la politique de la compagnie, vous devez reporter les enregistrements des zones d'ajustement entrepôt dans le grand livre article. Certaines compagnies choisissent de reporter quotidiennement les ajustements dans l'écriture article, alors que d'autres préfèrent effectuer une simulation de manière moins fréquente.

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Journal article**, puis sélectionnez le lien associé.  
2.  Renseignez les champs de chaque ligne journal.  
3.  Sélectionnez l'action **Calculer ajustement entrepôt** et renseignez les filtres selon vos besoins dans la fenêtre de demande de traitement en lot. Les ajustements sont calculés uniquement pour les écritures de la zone d'ajustement qui répondent aux exigences des filtres.  
4.  Sur le raccourci **Options**, entrez manuellement un numéro dans le champ **N° document**. Étant donné qu'aucune série de numéros n'a été configurée pour ce traitement en lot, utilisez le modèle de numéros configuré par l'entrepôt ou saisissez la date suivie de vos initiales.  
5.  Cliquez sur le bouton **OK**. Les ajustements positifs et négatifs sont totalisés pour chaque article, et les lignes sont créées dans le journal article pour les articles pour lesquels la somme est une quantité positive ou négative.  
6.  Reportez les lignes journal pour entrer les différences de quantité dans le grand livre article. L'inventaire des zones entrepôt correspond maintenant précisément à celui du grand livre article.  

## <a name="to-reclassify-an-items-lot-number"></a>Pour reclasser le numéro de lot d'un article
1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Feuilles reclassement article**, puis sélectionnez le lien connexe.
2. Dans la fenêtre **Feuilles reclassement article**, renseignez les champs selon vos besoins.
3. Dans le champ **N° lot**, saisissez le numéro de lot actuel de l'article.
4. Dans le champ **Nouveau N° lot**, saisissez le nouveau numéro de lot de l'article.
5. Sélectionnez l'action **Valider**.

Des phases spéciales s'appliquent lorsque vous souhaitez reclasser des numéros de série ou de lot. Pour plus d'informations, voir [Procédure : utiliser les numéros de lot et de série](inventory-how-work-item-tracking.md).

## <a name="see-also"></a>Voir aussi
[Inventaire](inventory-manage-inventory.md)
[Gestion d'entrepôt](warehouse-manage-warehouse.md)    
[Ventes](sales-manage-sales.md)  
[Procédure d'achat](purchasing-manage-purchasing.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

