---
title: "Créer des rapports d'analyse"
description: "Décrit comment créer de nouveaux rapports d'analyse pour les ventes, les achats et l'inventaire, et configurer des modèles d'analyse."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 06/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 72f1597eb226ee2a291b21faf83f582d6bdfa3f2
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
#  <a name="how-to-create-analysis-reports"></a>Procédure : créer des rapports d'analyse vente
Les directeurs des ventes doivent analyser de manière régulière le chiffre d'affaires, le profit bénéficiaire brut et d'autres indicateurs de performance des ventes clés. Les acheteurs, eux, s'intéressent plutôt à la dynamique des volumes d'achat, des performances des fournisseurs et des prix d'achat. Par ailleurs, les gestionnaires des inventaires et directeurs de la logistique ont besoin d'informations sur la rotation des inventaires, d'une analyse des mouvements d'inventaire et de statistiques sur la valeur d'inventaire.  

Vous pouvez utiliser des rapports d'analyse pour créer des rapports personnalisés basés sur les enregistrements de vos transactions reportées, comme les ventes, les achats, les transferts et les ajustements inventaire. Dans les rapports personnalisés, les données source, provenant du grand livre article (comportant des écritures valeur associées), peuvent être combinées, comparées et présentées de plusieurs manières, conformément aux souhaits de l'utilisateur. En ce sens, les rapports d'analyse sont très proches des rapports de tableau croisé dynamique de Microsoft Excel.  

Vous pouvez créer un rapport personnalisé consacré à vos comptes principaux, indiquant le chiffre d'affaires total (montants et quantités vendues), le profit bénéficiaire brut et le pourcentage de profit bénéficiaire brut du mois en cours, et comparer ces chiffres avec les résultats des mois précédents ou du même mois de l'année précédente, afin de calculer les écarts. Vous pouvez effectuer toutes ces opérations dans une seule et même vue, tout en ayant la possibilité d'accéder à chaque transaction pour rechercher la cause des zones problématiques identifiées en cliquant sur le bouton déroulant.  

Le rapport d'analyse contient les objets à analyser (par exemple, les clients, les groupes de clients, les représentants, etc.), représentés sous forme de lignes, et des paramètres d'analyse, qui déterminent la manière dont vous souhaitez analyser les objets, représentés sous forme de colonnes (par exemple, calculs de profit, comparaisons périodiques des volumes et des montants vente, ou comparaisons périodiques des chiffres réels et budgétés).

Outre les rapports d'analyse, vous pouvez créer et afficher des informations similaires dans des vues d'analyse, basées sur des axes analytiques. Pour plus d'informations, reportez vous à [Procédure : analyser des données par axe analytique](bi-how-analyze-data-dimension.md).

## <a name="example"></a>Exemple :  
Vous pouvez configurer les lignes suivantes :  
- Ordinateurs  
- Ecrans  
- Pièces de rechange  

Vous pouvez ensuite configurer les colonnes suivantes :  

- Ventes mois en cours  
- Ventes mois précédent  
- Ventes mois précédent (en %)  

## <a name="setting-up-line-and-column-layouts"></a>Configuration des présentations ligne et colonne  
 Dans la fenêtre **Rapport d'analyse**, vous pouvez afficher différentes présentations de ligne et de colonne selon le paramétrage effectué. Configurez vos lignes ou vos modèles de ligne dans la fenêtre **Modèles de ligne d'analyse**. Dans cette fenêtre, vous pouvez définir le nom du rapport et les objets à inclure dans les lignes du rapport. Configurez vos colonnes dans la fenêtre **Modèles de colonne d'analyse**. Dans cette fenêtre, vous pouvez définir le nom du modèle de colonne et les paramètres d'analyse à inclure dans le rapport sous forme de colonnes. Dans la fenêtre **Modèles de colonne d'analyse**, chaque ligne représente une colonne du rapport. Les lignes et les colonnes d'analyse sont indépendantes les unes des autres.  

Selon les lignes et les colonnes configurées, le programme totalise le résultat du rapport dans la fenêtre de la matrice **Rapport d'analyse** de ce type :  

|||||  
|-|-|-|-|  
||Ventes mois en cours|Ventes mois précédent|Ventes mois précédent (en %)|  
|Ordinateurs||||  
|Ecrans||||  
|Pièces de rechange||||  
|Total||||  

 Vous pouvez, par exemple, définir un jeu de lignes et plusieurs ensembles de présentations colonne afin d'afficher respectivement les rapports mensuel et annuel.

 ## <a name="to-set-up-analysis-column-templates"></a>Pour configurer des modèles de colonne d'analyse
La procédure suivante se base sur des vues d'analyse des ventes. Les étapes sont similaires aux vues d'analyse d'achat et d'inventaire.

Dans un rapport d'analyse, les paramètres d'analyse apparaissent sous forme de colonnes. Vous pouvez déterminer les colonnes à inclure dans le rapport d'analyse en configurant des modèles de colonne d'analyse.  

Un modèle contient un ensemble de lignes représentant les colonnes d'analyse du rapport d'analyse. Pour définir une colonne, attribuez un code type analyse à une ligne. Ce code type analyse détermine le type de données origine dans les écritures du grand livre d'articles sur lequel l'analyse est basée. Les données source incluent les coûts, le montant vente ou la quantité et leurs écritures valeur associées. Vous pouvez configurer autant de modèles de colonne que nécessaire, puis les utiliser pour créer des rapports d'analyse.    

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Modèles de colonne vente**, puis sélectionnez le lien connexe.  
2. Sélectionnez la première ligne vide, puis renseignez les champs selon vos besoins.
3. Sélectionnez l'action **Colonnes**.  
4. Dans la fenêtre **Colonnes d'analyse**, renseignez les champs afin d'indiquer les colonnes à inclure dans l'état d'analyse.  

    > [!NOTE]  
>   Pour définir une colonne, renseignez le champ **Code type analyse** de tous les types de colonne sauf **Formule**. Configurez les codes type analyse de la fenêtre **Types d'analyse**.  

    **Remarque**. Si vous sélectionnez **Ecritures article** dans le champ **Type écriture comptable**, les chiffres réels à partir de l'écriture comptable article sont copiés. Si vous sélectionnez **Ecritures budget article**, les chiffres budgétés à partir du budget sont copiés.  
5.  Cliquez sur le bouton **OK** pour enregistrer vos modifications.  

## <a name="to-set-up-analysis-line-templates"></a>Pour configurer des modèles de ligne d'analyse  
La procédure suivante se base sur des rapports d'analyse des ventes. Les étapes sont similaires aux rapports d'analyse d'achat et d'inventaire.

Dans un rapport d'analyse, les objets de l'analyse figurent sur les lignes. Vous pouvez déterminer les lignes à inclure dans le rapport d'analyse en configurant des modèles de ligne d'analyse.  

Les modèles contiennent un ensemble de lignes correspondant aux lignes d'analyse qui apparaissent dans le rapport d'analyse. Une ligne peut indiquer un ou plusieurs articles, clients, fournisseurs ou groupes. Vous pouvez également créer dans une ligne une formule totalisant les autres lignes. Vous pouvez configurer autant de modèles de ligne que nécessaire, puis les utiliser pour créer des rapports d'analyse.    

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Modèles de ligne vente**, puis sélectionnez le lien connexe.  
2. Sélectionnez la première ligne vide, puis renseignez les champs selon vos besoins.
3. Sélectionnez l'option **Lignes**.  
4. Dans la fenêtre **Ligne d'analyse**, créez des lignes pour les articles, clients, fournisseurs ou vendeurs dont vous voulez voir les chiffres dans votre état d'analyse. Vous devez renseigner les champs **Type**, **Plage** et **Désignation**.  

> [!NOTE]  
>   Lorsque vous voulez créer plusieurs lignes distinctes pour chaque article, client, etc., vous pouvez également sélectionner l'option d'insertion appropriée pour renseigner tous les champs pertinents de la ligne. Si vous le souhaitez, vous pouvez alors modifier les lignes manuellement. Pour insérer des lignes, choisissez **Insérer des articles** ou **Insérer des groupes articles**.  

## <a name="to-create-a-new-sales-analysis-report"></a>Pour créer un rapport d'analyse vente
La procédure suivante se base sur des rapports d'analyse des ventes. Les étapes sont similaires aux rapports d'analyse d'achat et d'inventaire.

Les rapports d'analyse permettent d'analyser la dynamique de vos ventes en fonction des indicateurs de performances des ventes clés que vous sélectionnez, par exemple le volume des ventes en matière de montant et de quantité, la marge contributive ou l'évolution des ventes réelles par rapport au budget. Ils peuvent également servir à analyser vos prix de vente moyens et à évaluer les performances de vos commerciaux.  

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "Page ou état pour la recherche"), entrez **Rapports d'analyse vente**, puis sélectionnez le lien connexe.  
2. Dans la fenêtre **Rapports d'analyse vente**, cliquez sur l'action **Nouveau**.
3. Renseignez les champs selon vos besoins. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Choisissez l'action **Modifier le rapport d'analyse**.
5. Dans la fenêtre **Rapports d'analyse vente**, cliquez sur l'action **Afficher matrice**.  

> [!NOTE]  
>   Si vous le souhaitez, vous pouvez mettre au point des combinaisons de modèles de ligne et de colonne pour créer des états et leur affecter des noms uniques. Dans ce cas, en sélectionnant le nom d'un état, vous n'aurez pas à sélectionner des modèles de ligne et de colonne dans la fenêtre **Rapport d'analyse vente**. Une fois que vous avez choisi un nom de rapport, vous pouvez changer individuellement les modèles de ligne et de colonne et ensuite sélectionner une nouvelle fois le nom du rapport afin de restaurer la combinaison d'origine.

## <a name="see-also"></a>Voir aussi
[Veille économique](bi.md)  
[Finances](finance.md)  
[Configuration de Finance](finance-setup-finance.md)  
[Les écritures comptables et le plan comptable](finance-general-ledger.md)  
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

