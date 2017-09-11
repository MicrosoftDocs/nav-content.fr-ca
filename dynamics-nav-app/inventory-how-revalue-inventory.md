<properties
                pageTitle="Procédure : Réévaluer l'inventaire | Dynamics NAV"
                description="Décrit comment réévaluer ou amortir la valeur d'un ou de plusieurs articles en inventaire en reportant leur valeur calculée actuelle."
                services="project-madeira"
                documentationCenter=""
                authors="SorenGP"
/>
<tags
    ms.service="project-madeira"
    ms.topic="article"
    ms.devlang="na"
    ms.tgt_pltfrm="na"
    ms.workload="na"
    ms.date="11/07/2016"
    ms.author="SorenGP" />


# <a name="how-to-revalue-inventory"></a><span data-ttu-id="fe4f1-103">Procédure : réévaluer l'inventaire</span><span class="sxs-lookup"><span data-stu-id="fe4f1-103">How to: Revalue Inventory</span></span>   
<span data-ttu-id="fe4f1-104">Pour réévaluer ou amortir un article ou une écriture article spécifique, vous devez utiliser le journal réévaluation.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span></span>

## <a name="to-revalue-inventory"></a><span data-ttu-id="fe4f1-105">Pour réévaluer l'inventaire</span><span class="sxs-lookup"><span data-stu-id="fe4f1-105">To revalue inventory</span></span>
1. <span data-ttu-id="fe4f1-106">Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, entrez **Feuille réévaluation**, puis sélectionnez le lien connexe.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Revaluation Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="fe4f1-107">Choisissez l'action **Calculer valeur stock**.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-107">Choose the **Calculate Inventory Value** action.</span></span>
3. <span data-ttu-id="fe4f1-108">Dans la fenêtre **Calculer valeur stock**, renseignez les champs selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-108">In the **Calculate Inventory Value** window, fill in the fields as necessary.</span></span> <span data-ttu-id="fe4f1-109">Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-109">Choose a field to read a short description of the field or link to more information.</span></span>
4. <span data-ttu-id="fe4f1-110">Cliquez sur le bouton **OK**.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-110">Choose the **OK** button.</span></span>
5. <span data-ttu-id="fe4f1-111">Sur chaque ligne de la fenêtre **Feuille réévaluation**, indiquez le nouveau coût unitaire dans le champ **Coût unitaire (réévalué)**.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-111">On each line in the **Revaluation Journal** window, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span></span> <span data-ttu-id="fe4f1-112">Vous pouvez aussi indiquer le nouveau montant total dans le champ **Valeur stock (réévaluée)**.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-112">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span></span>

    <span data-ttu-id="fe4f1-113">Les champs appropriés sont automatiquement mis à jour.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-113">The relevant fields are automatically updated.</span></span> <span data-ttu-id="fe4f1-114">Remarque : le champ **Montant** affiche la modification réelle de la valeur du stock pour l'écriture comptable article sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-114">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span></span> <span data-ttu-id="fe4f1-115">Il calcule la différence entre les champs **Valeur stock (calculée)** et **Valeur stock (réévaluée)**.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-115">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span></span>

6. <span data-ttu-id="fe4f1-116">Lorsque vous avez renseigné toutes les lignes de la feuille réévaluation, choisissez l'action **Valider**.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-116">When you have completed all lines in the revaluation journal, choose the **Post** action.</span></span>

<span data-ttu-id="fe4f1-117">Les nouvelles écritures valeur sont alors créées pour refléter les appréciations que vous avez reportées.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-117">New value entries are now created to reflect the revaluations that you have posted.</span></span> <span data-ttu-id="fe4f1-118">Vous pouvez visualiser les nouvelles valeurs dans les fiches article concernées.</span><span class="sxs-lookup"><span data-stu-id="fe4f1-118">You can see the new values on the respective item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="fe4f1-119">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fe4f1-119">See Also</span></span>
[<span data-ttu-id="fe4f1-120">Gestion du stock</span><span class="sxs-lookup"><span data-stu-id="fe4f1-120">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="fe4f1-121">Gestion des ventes</span><span class="sxs-lookup"><span data-stu-id="fe4f1-121">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="fe4f1-122">Gestion des achats</span><span class="sxs-lookup"><span data-stu-id="fe4f1-122">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="fe4f1-123">Utiliser Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="fe4f1-123">Work With Dynamics NAV</span></span>](ui-work-product.md)

