---
title: "Pratiques recommandées pour la configuration globale de la planification"
description: "Le raccourci **Planification** de la fenêtre **Configuration de la fabrication** comporte plusieurs champs permettant de définir des règles globales pour la planification de l'approvisionnement."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b6437c809af79c1c0c24126aaa38e6da6120d066
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="setup-best-practices-global-planning-setup"></a>Pratiques de configuration recommandées : configuration globale de la planification
Le raccourci **Planning** de la fenêtre**Paramètres production** comporte plusieurs champs permettant de définir les règles globales pour la planification des approvisionnements.  

 Le tableau suivant fournit les meilleures pratiques sur la procédure de configuration de champs paramètres sélectionnés de planification générale. Pour plus d'informations sur un champ donné, sélectionnez le lien correspondant dans la colonne **Configuration d'un champ**.  

|Champ de configuration|Meilleure pratique|Commentaire|  
|-----------------|-------------------|-------------|  
|Prévision sur magasin|Indiquez si vous avez des prévisions pour des entrepôts spécifiques.||  
|Mag. composant par déf.|Si les articles ne sont pas définis comme unités de stock, sélectionnez le code d'emplacement de l'entrepôt principal.|Cela s'applique également si vous utilisez uniquement la feuille de réquisition.|  
|Niveau de dépassement de capacité vide|Sélectionnez **Autoriser calcul par défaut** si vous effectuez une migration de Microsoft Dynamics NAV 5.0 ou d'une version antérieure.|Ne l'utilisez que si vous souhaitez autoriser tout ou partie de vos articles à franchir le point de réapprovisionnement.|  
|Période tampon par défaut|Doit être compris entre 1D et 5D.<br /><br /> Si vous débutez en planification avec [!INCLUDE[d365fin](includes/d365fin_md.md)], définissez une plus longue période.|Quand les utilisateurs sont plus au fait des différents motifs des messages d'action, raccourcissez la période tampon pour autoriser plus de propositions de modification.|  
|Quantité tampon par défaut|Définissez à entre 5 et 20 % de la taille du lot de l'article.||  

## <a name="see-also"></a>Voir aussi  
 [Pratiques de configuration recommandées : planification de l'approvisionnement](setup-best-practices-supply-planning.md)   
 [Détails de conception : planification de l'approvisionnement](design-details-supply-planning.md)   
 [Configurez les modules complexes à l'aide des meilleures pratiques](set-up-complex-application-areas-using-best-practices.md)  
 [Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

