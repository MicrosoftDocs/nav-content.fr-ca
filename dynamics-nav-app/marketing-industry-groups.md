---
title: "Configurer des secteurs d'activité pour des compagnies contact"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 5d0a8f8f8f1e5b50671911d6bfba3da00f2d7ae2
ms.contentlocale: fr-ca
ms.lasthandoff: 07/19/2017

---
# <a name="set-up-industry-groups-for-contact-companies"></a><span data-ttu-id="8b2e7-102">Configurer des secteurs d'activité pour des compagnies contact</span><span class="sxs-lookup"><span data-stu-id="8b2e7-102">Set Up Industry Groups for Contact Companies</span></span>
<span data-ttu-id="8b2e7-103">Les secteurs d'activité vous permettent d'indiquer le type de secteur auquel vos contacts appartiennent, par exemple la grande distribution et l'industrie automobile.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-103">You use industry groups to indicate the type of industry to which your contacts belong, for example, the retail industry or the automobile industry.</span></span>

<span data-ttu-id="8b2e7-104">L'utilisation secteurs d'activité sur les contacts est un processus en deux étapes.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-104">Using industry groups on contacts is a two-step process.</span></span> <span data-ttu-id="8b2e7-105">Tout d'abord, vous définissez le code secteur d'activité.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-105">First, you define the industry group code.</span></span> <span data-ttu-id="8b2e7-106">Vous ne devez effectuer cette étape qu'une seule fois pour chaque secteur d'activité.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-106">You only have to perform this step one time for each industry group.</span></span> <span data-ttu-id="8b2e7-107">Une fois que vous disposez d'un code secteur d'activité, vous pouvez commencer à affecter ce code aux compagnies contact.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-107">Once you have an industry group code, you can start to assign the code to contact companies.</span></span>

<span data-ttu-id="8b2e7-108">**Remarque** : si vous prévoyez de synchroniser vos contacts avec des fournisseurs, des clients ou des comptes bancaires dans d'autres parties de l'application, vous pouvez configurer pour eux une relation d'affaires.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-108">**Note:** If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="define-an-industry-group-code"></a><span data-ttu-id="8b2e7-109">Définir un code secteur d'activité</span><span class="sxs-lookup"><span data-stu-id="8b2e7-109">Define an Industry Group Code</span></span>
<span data-ttu-id="8b2e7-110">Le code secteur d'activité définit le type ou la catégorie du groupe, par exemple PUB pour la publicité, ou PRESSE pour la télévision et la radio.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-110">The industry group code defines the type or category of the group, such as ADVERT for advertising, or PRESS, for TV and radio.</span></span> <span data-ttu-id="8b2e7-111">Vous pouvez disposer de plusieurs codes secteur d'activité.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-111">You can have several industry group codes.</span></span> <span data-ttu-id="8b2e7-112">Pour définir les secteurs d'activité, utilisez la fenêtre **Secteurs d'activité**.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-112">To define the industry groups, you use the **Industry Groups** window.</span></span>

1. <span data-ttu-id="8b2e7-113">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Secteurs d'activité**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-113">In the top right corner, choose the **Search for Page or Report** icon, enter **Industry Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="8b2e7-114">Sélectionnez l'action **Nouveau**, et entrez un code et une description.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-114">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="8b2e7-115">Vous pouvez saisir pour le code un maximum de 11 caractères, et toute combinaison de chiffres et des lettres.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-115">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="assign-industry-groups-to-a-contact"></a><span data-ttu-id="8b2e7-116">Affecter des secteurs d'activité à un contact</span><span class="sxs-lookup"><span data-stu-id="8b2e7-116">Assign Industry Groups to a Contact</span></span>
<span data-ttu-id="8b2e7-117">Vous ne pouvez pas affecter de secteurs d'activité à une personne contact, mais uniquement à des compagnies.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-117">You cannot assign industry groups to a contact person - only companies.</span></span>

1. <span data-ttu-id="8b2e7-118">Ouvrez le contact.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-118">Open the contact.</span></span>
2. <span data-ttu-id="8b2e7-119">Sélectionnez l'action **Société**, puis l'action **Secteurs d'activité**.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-119">Choose the **Company** action, and then the **Industry Groups** action.</span></span> <span data-ttu-id="8b2e7-120">La fenêtre **Secteur d'activité contact** s'affiche.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-120">The **Contact Industry Groups** window opens.</span></span>
3. <span data-ttu-id="8b2e7-121">Dans le champ **Code secteurs d'activité**, sélectionnez le secteur d'activité à affecter.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-121">In the **Industry Groups Code** field, select the industry groups you want to assign.</span></span>

<span data-ttu-id="8b2e7-122">Répétez ces étapes pour chaque secteur d'activité à affecter.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-122">Repeat these steps to assign as many industry groups as you want.</span></span> <span data-ttu-id="8b2e7-123">Vous pouvez également affecter des secteurs d'activité à partir de la liste des contacts en suivant la même procédure.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-123">You can also assign industry groups from the contact list by following the same procedure.</span></span>

<span data-ttu-id="8b2e7-124">Le nombre de secteurs d'activité que vous avez affectés au contact s'affiche dans le champ **Nbre secteurs d'activité** de la section **Segmentation** de la fenêtre **Contact**.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-124">The number of industry groups that you have assigned to the contact is displayed in the **No. of Industry Groups** field on the **Segmentation** section of the **Contact** window.</span></span>

<span data-ttu-id="8b2e7-125">Une fois que vous avez affecté des secteurs d'activité à vos contacts, vous pouvez utiliser ces informations pour sélectionner des contacts pour vos segments.</span><span class="sxs-lookup"><span data-stu-id="8b2e7-125">After you have assigned industry groups to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="8b2e7-126">Pour plus d'informations, reportez-vous à [Procédure : ajouter des contacts à des segments](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="8b2e7-126">For more information, see [How to: Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="8b2e7-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8b2e7-127">See Also</span></span>
[<span data-ttu-id="8b2e7-128">Création de sociétés contact</span><span class="sxs-lookup"><span data-stu-id="8b2e7-128">Create Contact Companies</span></span>](marketing-create-contact-companies.md)

