---
title: Dimensions
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a1b38e74717e87bea6efb46f8f4e5236b6ec4e64
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---

#<a name="dimensions"></a>Dimensions
Les axes sont des données que vous ajoutez aux écritures pour les catégoriser à des fins d'analyse. Par exemple, certains axes peuvent indiquer de quel projet ou département provient une écriture.
Vous pouvez alors utiliser les axes analytiques au lieu de configurer des comptes généraux distincts pour chaque département et projet. Cela vous permet d'avoir des informations d'analyse riches dans vos données sans avoir besoin d'utiliser un plan comptable complexe.
Vous pouvez définir un nombre d'axes illimité avec un nombre de sections analytiques illimité.  

Par exemple, vous configurez un axe analytique appelé *Département*, et vous utilisez cet axe et une section analytique lorsque vous validez des documents vente. Ensuite, vous pouvez ultérieurement obtenir les données de veille économique, par exemple sur quels articles ont été vendus par quels départements.
Plus vous configurez et utilisez d'axes analytiques, plus vous pouvez baser vos décisions commerciales sur des états détaillés. Par exemple, une seule écriture vente peut comporter plusieurs informations de dimension : le compte sur lequel la vente de l'article a été reportée, l'endroit où l'article a été vendu, le nom du vendeur et le type de client qui a effectué l'achat.  

## <a name="using-dimensions"></a>Utilisation des axes analytiques
Dans un document tel qu'un document de vente, vous pouvez ajouter des informations de dimension pour une seule ligne document et pour le document lui-même. Par exemple, dans la fenêtre **Commande vente**, vous pouvez saisir des sections analytiques pour les deux premiers raccourcis axe directement dans le document et ajouter des informations analytiques complémentaires si vous cliquez sur le bouton **Axes analytiques**.  
Si vous travaillez plutôt sur un journal, vous pouvez également ajouter à une écriture des informations de dimension de la même manière, si vous avez configuré des raccourcis dimension en tant que champs directement dans les lignes journal.  
Vous pouvez configurer des axes analytiques par défaut pour des comptes ou des types de compte, de sorte que les axes et les sections analytiques soient renseignés automatiquement.  

## <a name="dimension-sets"></a>Ensembles de dimensions
Un ensemble de dimensions est une combinaison unique de sections analytiques. Il est stocké comme des écritures de l'ensemble de dimensions dans la base de données. Chaque écriture de l'ensemble de dimensions représente une valeur de dimension unique. L'ensemble de dimensions est identifié par un code commun, qui est affecté à chaque écriture correspondante qui appartient à l'ensemble de dimensions.  

Lorsque vous créez une ligne de journal, un en-tête de document ou une ligne de document, vous pouvez spécifier une combinaison de valeurs de dimension. Au lieu d'enregistrer explicitement chaque valeur de dimension dans la base de données, un code d'ensemble de dimensions est affecté à la ligne de journal, à l'en-tête du document ou à la ligne du document pour spécifier l'ensemble de dimensions.  

## <a name="see-also"></a>Voir aussi
[Finance](finance-setup.md)  
[Configuration des axes analytiques](finance-setup-setup-dimensions.md)  

