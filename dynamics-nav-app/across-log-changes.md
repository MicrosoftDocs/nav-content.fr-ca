---
title: "Effectuer le suivi de l'activité utilisateur dans un journal modification"
Description: "Vous pouvez activer un journal utilisateur de sorte que vous avez un historique de toutes les modifications apportées aux données dans les tables suivies."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 74d70c9929cfa29909281b964488319be7a9f127
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---
# <a name="logging-changes-in-dynamics-nav"></a>Journalisation des modifications dans Dynamics NAV
Vous pouvez activer le journal des modifications dans [!INCLUDE[d365fin](includes/d365fin_md.md)] afin d'avoir un historique des activités. Le journal est basé sur les modifications apportées aux données dans les tableaux que vous suivez. Dans le journal des modifications, les entrées sont chronologiquement ordonnées et montrent les modifications apportées aux champs des tables spécifiées. Le journal modification regroupe tous les changements apportés à la table.  

## <a name="working-with-the-change-log"></a>Utilisation du journal des modifications
Dans de nombreux systèmes financiers, il est souvent difficile de trouver l'origine des erreurs ou des modifications de données. Il peut s'agir d'une simple erreur de numéro de téléphone client comme d'une écriture erronée. Le journal des modifications vous permet de suivre toutes les modifications directes apportées par un utilisateur aux données dans la base de données. Vous devez spécifier les opérations que le système doit journaliser, pour chaque table et chaque champ, puis activer le journal modification.  

Vous devez activer et désactiver le journal des modifications dans la fenêtre **Paramètres journal modification**. Lorsque vous activez ou désactivez le journal des modifications, cette activité est enregistrée, ainsi vous pouvez toujours savoir quel utilisateur est à l'origine de la modification Cette fonction ne peut pas être désactivée.  

Dans la fenêtre **Configuration journal modif.**, si vous choisissez l'action **Tables**, vous pouvez spécifier les tables dont vous souhaitez suivre les modifications, et quelles modifications suivre. [!INCLUDE[d365fin](includes/d365fin_md.md)] suit également un nombre de tables système.

Une fois que vous avez configuré et activé le journal des modifications et modifié des données, vous pouvez afficher et filtrer les modifications dans la fenêtre **Écritures journal modification**. Vous pouvez supprimer des données à partir de la fenêtre **Suppr écritures journal modif**, dans laquelle vous pouvez définir des filtres basés sur la date et l'heure.  

## <a name="see-also"></a>Voir aussi
[Modification des paramètres de base](ui-change-basic-settings.md)  
[Tri](ui-sorting.md)  
[Utilisation de l'icône Page ou état pour la recherche](ui-search.md)  
[Procédure : gérer les utilisateurs et les autorisations](ui-how-users-permissions.md)    
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

