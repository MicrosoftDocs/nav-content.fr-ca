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
# <a name="logging-changes-in-dynamics-nav"></a><span data-ttu-id="0fb0e-103">Journalisation des modifications dans Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="0fb0e-103">Logging Changes in Dynamics NAV</span></span>
<span data-ttu-id="0fb0e-104">Vous pouvez activer le journal des modifications dans [!INCLUDE[d365fin](includes/d365fin_md.md)] afin d'avoir un historique des activités.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-104">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span></span> <span data-ttu-id="0fb0e-105">Le journal est basé sur les modifications apportées aux données dans les tableaux que vous suivez. Dans le journal des modifications, les entrées sont chronologiquement ordonnées et montrent les modifications apportées aux champs des tables spécifiées.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-105">The log is based on changes that are made to data in the tables that you track. In the change log, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span></span> <span data-ttu-id="0fb0e-106">Le journal modification regroupe tous les changements apportés à la table.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-106">The change log collects all changes that are made to the table.</span></span>  

## <a name="working-with-the-change-log"></a><span data-ttu-id="0fb0e-107">Utilisation du journal des modifications</span><span class="sxs-lookup"><span data-stu-id="0fb0e-107">Working with the change log</span></span>
<span data-ttu-id="0fb0e-108">Dans de nombreux systèmes financiers, il est souvent difficile de trouver l'origine des erreurs ou des modifications de données.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-108">A common problem in many financial systems is to locate the origin of errors and changes in data.</span></span> <span data-ttu-id="0fb0e-109">Il peut s'agir d'une simple erreur de numéro de téléphone client comme d'une écriture erronée.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-109">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span></span> <span data-ttu-id="0fb0e-110">Le journal des modifications vous permet de suivre toutes les modifications directes apportées par un utilisateur aux données dans la base de données.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-110">The change log lets you track all direct modifications a user makes to data in the database.</span></span> <span data-ttu-id="0fb0e-111">Vous devez spécifier les opérations que le système doit journaliser, pour chaque table et chaque champ, puis activer le journal modification.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-111">You must specify each table and field that you want the system to log, and then you must activate the change log.</span></span>  

<span data-ttu-id="0fb0e-112">Vous devez activer et désactiver le journal des modifications dans la fenêtre **Paramètres journal modification**.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-112">You activate and deactivate the change log in the **Change Log Setup** window.</span></span> <span data-ttu-id="0fb0e-113">Lorsque vous activez ou désactivez le journal des modifications, cette activité est enregistrée, ainsi vous pouvez toujours savoir quel utilisateur est à l'origine de la modification</span><span class="sxs-lookup"><span data-stu-id="0fb0e-113">When you activate or deactivate the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span></span> <span data-ttu-id="0fb0e-114">Cette fonction ne peut pas être désactivée.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-114">This cannot be turned off.</span></span>  

<span data-ttu-id="0fb0e-115">Dans la fenêtre **Configuration journal modif.**, si vous choisissez l'action **Tables**, vous pouvez spécifier les tables dont vous souhaitez suivre les modifications, et quelles modifications suivre. [!INCLUDE[d365fin](includes/d365fin_md.md)] suit également un nombre de tables système.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-115">In the **Change Log Setup** window, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span></span>

<span data-ttu-id="0fb0e-116">Une fois que vous avez configuré et activé le journal des modifications et modifié des données, vous pouvez afficher et filtrer les modifications dans la fenêtre **Écritures journal modification**.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-116">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes in the **Change Log Entries** window.</span></span> <span data-ttu-id="0fb0e-117">Vous pouvez supprimer des données à partir de la fenêtre **Suppr écritures journal modif**, dans laquelle vous pouvez définir des filtres basés sur la date et l'heure.</span><span class="sxs-lookup"><span data-stu-id="0fb0e-117">If you want to delete entries, you can do that in the **Delete Change Log Entries** window, where you can set filters based on dates and time.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0fb0e-118">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0fb0e-118">See Also</span></span>
[<span data-ttu-id="0fb0e-119">Modification des paramètres de base</span><span class="sxs-lookup"><span data-stu-id="0fb0e-119">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="0fb0e-120">Tri</span><span class="sxs-lookup"><span data-stu-id="0fb0e-120">Sorting</span></span>](ui-sorting.md)  
[<span data-ttu-id="0fb0e-121">Utilisation de l'icône Page ou état pour la recherche</span><span class="sxs-lookup"><span data-stu-id="0fb0e-121">Using Search for Page or Report</span></span>](ui-search.md)  
<span data-ttu-id="0fb0e-122">[Procédure : gérer les utilisateurs et les autorisations](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="0fb0e-122">[How to: Manage Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="0fb0e-123">[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0fb0e-123">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

