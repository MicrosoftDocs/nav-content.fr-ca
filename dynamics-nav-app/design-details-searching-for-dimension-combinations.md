---
title: "Détails de conception - Recherche des combinaisons de dimensions"
description: "Lorsque vous fermez une fenêtre après avoir modifié un ensemble de dimensions, [!INCLUDE[d365fin](includes/d365fin_md.md)] évalue si l'ensemble de dimensions modifié existe. Si l'ensemble n'existe pas, un nouvel ensemble est créé et le code de combinaisons de dimensions est retourné."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1e3bbad5d5f809068b88f6bbf5d0deaa22b38427
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-searching-for-dimension-combinations"></a>Détails de conception : recherche des combinaisons de dimensions
Lorsque vous fermez une fenêtre après avoir modifié un ensemble de dimensions, [!INCLUDE[d365fin](includes/d365fin_md.md)] évalue si l'ensemble de dimensions modifié existe. Si l'ensemble n'existe pas, un nouvel ensemble est créé et le code de combinaisons de dimensions est retourné.  

## <a name="building-search-tree"></a>Création d'un arbre de recherche  
 La table 481 **Nœud d'arbre ensemble de dimensions** est utilisé lorsque [!INCLUDE[d365fin](includes/d365fin_md.md)] évalue si un ensemble de dimensions existe déjà dans la table **Écriture de l'ensemble de dimensions** de la table 480. L'évaluation est exécutée en parcourant de manière récursive l'arbre de recherche en commençant par le niveau numéroté 0. Le plus haut niveau 0 représente un ensemble de dimensions sans les écritures d'ensemble de dimensions. Les enfants cet ensemble de dimensions représentent des ensembles de dimensions avec une seule écriture d'ensemble de dimensions. Les enfants de ces ensembles de dimensions représentent des ensembles de dimensions avec deux enfants, etc.  

### <a name="example-1"></a>Exemple 1  
 Le schéma suivant représente un arbre de recherche avec six ensembles de dimensions. Seule l'écriture d'ensemble de dimensions distinctive est affichée dans le schéma.  

 ![Structure arborescente des dimensions](media/nav2013_dimension_tree.png "NAV2013_Dimension_Tree")  

 Le tableau suivant décrit une liste complète des écritures d'ensemble de dimensions qui constituent chaque ensemble de dimensions.  

|Ensembles de dimensions|Écritures de l'ensemble de dimensions|  
|--------------------|---------------------------|  
|Ensemble 0|Aucun|  
|Ensemble 1|AREA 30|  
|Ensemble 2|AREA 30, DEPT ADM|  
|Ensemble 3|AREA 30, DEPT PROD|  
|Ensemble 4|AREA 30, DEPT ADM, PROJ VW|  
|Ensemble 5|AREA 40|  
|Ensemble 6|AREA 40, PROJ VW|  

### <a name="example-2"></a>Exemple 2  
 Cet exemple montre la manière dont [!INCLUDE[d365fin](includes/d365fin_md.md)] évalue si un ensemble de dimensions constitué des écritures de l'ensemble de dimensions AREA 40, DEPT PROD existe.  

 D'abord, [!INCLUDE[d365fin](includes/d365fin_md.md)] met également à jour la table **Nœud d'arbre ensemble de dimensions** pour s'assurer que l'arbre de recherche ressemble au schéma suivant. Ainsi, l'ensemble de dimensions 7 devient un enfant de l'ensemble de dimensions 5.  

 ![NAV2013&#95;Dimension&#95;Tree&#95;Example 2](media/nav2013_dimension_tree_example2.png "NAV2013_Dimension_Tree_Example2")  

### <a name="finding-dimension-set-id"></a>Recherche du code ensemble de dimensions  
 Au niveau conceptuel, **Code parent**, **Dimension** et **Section analytique**, dans l'arbre de recherche, sont combinés et sont utilisés comme clé primaire, car [!INCLUDE[d365fin](includes/d365fin_md.md)] parcourt l'arborescence dans le même ordre que les écritures analytiques. La fonction GET (enregistrement) est utilisée pour rechercher le code de l'ensemble de dimensions L'exemple de code suivant indique comment trouver le code d'ensemble de dimensions lorsqu'il existe trois valeurs de dimension.  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet."Parent ID",UserDim.DimCode,UserDim.DimValueCode);  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

 Toutefois, pour préserver la capacité de [!INCLUDE[d365fin](includes/d365fin_md.md)] de renommer un axe et une section analytique, la table 348 **Section analytique** est étendue avec un champ d'entier **ID section analytique**. Ce tableau convertit la paire de champs **Axe analytique** et **Section analytique** sur une valeur entière. Lorsque vous renommez la dimension et la valeur de dimension, la valeur d'entier n'est pas modifiée.  

```  
DimSet."Parent ID" := 0;  // 'root'  
IF UserDim.FINDSET THEN  
  REPEAT  
      DimSet.GET(DimSet.ParentID,UserDim."Dimension Value ID");  
  UNTIL UserDim.NEXT = 0;  
EXIT(DimSet.ID);  

```  

## <a name="see-also"></a>Voir aussi  
 [Fonction GET (Enregistrement)](https://msdn.microsoft.com/en-us/library/dd301056.aspx)    
 [Détails de conception : écritures d'ensemble de dimensions](design-details-dimension-set-entries.md)   
 [Aperçu des écritures de l'ensemble de dimensions](design-details-dimension-set-entries-overview.md)   
 [Détails de conception : structure de la table](design-details-table-structure.md)   
 [Détails de conception : Codeunit 408 Gestion des dimensions](design-details-codeunit-408-dimension-management.md)   
 [Détails de conception : exemples de code de motifs modifiés dans les modifications](design-details-code-examples-of-changed-patterns-in-modifications.md)

