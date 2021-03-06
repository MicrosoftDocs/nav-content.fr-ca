---
title: "Consolider les données de plusieurs compagnies"
description: "Obtenez une vue récapitulative de la santé financière de vos entreprises."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: consolidation, subsidiaries, consolidate
ms.date: 07/14/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f1590afe99c5cea9a70e580445014ff4e25dccee
ms.contentlocale: fr-ca
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-work-with-the-consolidated-trial-balance-report"></a>Procédure : utiliser le rapport Balance de vérification consolidé
Si vous avez plusieurs compagnies dans [!INCLUDE[d365fin](includes/d365fin_md.md)], le rapport Balance de vérification consolidée du tableau de bord Comptable peut vous donner un aperçu de leur santé financière dans leur ensemble.  

Le rapport regroupe les écritures grand livre de chacune de vos compagnies dans une nouvelle compagnie que vous créez pour stocker les données consolidées. Cette compagnie est généralement appelée « compagnie consolidée ». La compagnie consolidée est un simple conteneur pour les données consolidées, et ne contient pas de données métier en temps réel. Les compagnies que vous incluez dans la compagnie consolidée deviennent des **Unités fonctionnelles** dans le rapport.

Vous pouvez consolider :  

* entre compagnies ayant plusieurs plans comptables ;  
* des compagnies qui utilisent plusieurs exercices financiers et devises ;  
* la totalité ou un pourcentage des informations financières d'une compagnie ;
* Utilisation de plusieurs taux de change dans des comptes du grand livre individuels 

En fonction de la complexité de vos activités, il existe deux façons de configurer le rapport :

* Si les paramètres avancés ne sont pas nécessaires, par exemple l'ajout d'une compagnie que vous détenez en partie, vous pouvez utiliser le guide de configuration assistée **Consolidation de la compagnie** pour configurer rapidement une consolidation. Le guide vous aide à effectuer les étapes de base.
* Si d'autres paramètres avancés sont nécessaires, vous pouvez configurer vous-même la compagnie consolidée et les unités fonctionnelles.

## <a name="to-do-a-simple-consolidation-setup"></a>Pour configurer une consolidation simple 
Si votre consolidation est simple, car vous détenez en totalité les unités fonctionnelles à consolider, le guide de configuration assistée **Consolidation de la compagnie** vous aide à effectuer les étapes suivantes :
  
* Choisissez si vous souhaitez créer une compagnie consolidée, ou consolider les données dans une compagnie que vous avez déjà créée pour la consolidation. La compagnie ne doit pas contenir de transactions.
* Affichez un aperçu des résultats. [!INCLUDE[d365fin](includes/d365fin_md.md)] vérifie que les données de base et les transactions peuvent être transférées avec succès vers la compagnie consolidée.

Pour utiliser le guide de configuration assistée, procédez comme suit :

1. Dans le tableau de bord **Comptable**, choisissez l'action **Configuration assistée**.
2. Choisissez **Configurer la génération de rapports de consolidation**, puis effectuez chaque étape du guide de configuration assistée.

## <a name="to-do-an-advanced-consolidation-setup"></a>Pour configurer une consolidation avancée
Si des paramètres plus avancés sont nécessaires pour votre consolidation, vous pouvez configurer manuellement la consolidation. Par exemple, si vous détenez partiellement des compagnies, ou si vous ne souhaitez pas inclure des compagnies dans la consolidation. Vous configurez la compagnie consolidée de la même manière que vous configurez d'autres compagnies. Pour plus d'informations, voir [Préparation aux activités commerciales](ui-get-ready-business.md).  

[!INCLUDE[d365fin](includes/d365fin_md.md)] vous permet de configurer une liste de compagnies à consolider, de vérifier les données comptables avant leur consolidation, d'importer des fichiers et de générer des rapports de consolidation.  

1. Connectez-vous à la compagnie consolidée.
2. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Unités fonctionnelles**, puis sélectionnez le lien associé.  
3. Sélectionnez **Nouveau**, puis renseignez les champs requis.  

Si votre unité fonctionnelle utilise une devise étrangère, indiquez le taux de change à utiliser dans la consolidation. Vous devez également entrer des informations de consolidation sur les comptes du grand livre de l'unité fonctionnelle. Ces processus sont décrits dans les sections suivantes.

### <a name="to-prepare-general-ledger-accounts-for-consolidation"></a>Pour préparer les comptes GL pour la consolidation 
Si le plan comptable de l'unité fonctionnelle diffère de celui de la compagnie consolidée, vous devez préparer les comptes GL pour la consolidation. Vous pouvez spécifier les comptes sur lesquels reporter les débits et crédits et la méthode à utiliser pour convertir des devises dans la compagnie consolidée. Par exemple, cela est utile si vous exécutez souvent le rapport.

1. Sélectionnez l'icône ![Page ou état pour la recherche](media/ui-search/search_small.png "icône Page ou état pour la recherche"), entrez **Plan comptable**, puis sélectionnez le lien connexe.  
2. Ouvrez la fiche du compte, puis renseignez les champs du raccourci **Consolidation**.

### <a name="to-specify-exchange-rates-for-consolidations"></a>Pour indiquer des taux de change pour les consolidations
Si une unité fonctionnelle utilise une devise différente de celle de la compagnie consolidée, vous devez spécifier des méthodes de conversion de taux de change pour chaque compte avant la consolidation. Pour chaque compte, la valeur du champ **Consolider la méthode de traduction** détermine le taux de change. Dans chaque fiche unité fonctionnelle, dans le champ **Table Taux de change devise**, vous spécifiez si la consolidation utilise les taux de change de l'unité fonctionnelle ou de la compagnie consolidée. Si vous utilisez les taux de change de la compagnie consolidée, vous pouvez les modifier pour une unité fonctionnelle. Pour les unités fonctionnelles, si le champ **Table Taux de change devise** de la fiche unité fonctionnelle contient la valeur **Local**, vous pouvez modifier le taux de change à partir de la fiche unité fonctionnelle. Les taux de change sont copiés à partir de la table **Taux de change devise**, mais vous pouvez les modifier avant la consolidation. 

Le tableau suivant décrit les méthodes de conversion de taux de change que vous pouvez utiliser pour les comptes.

|Taux de change | Utilisation courante |
|---|---|
|Taux moyen (manuel) | Vous calculez manuellement le taux moyen pour la période à consolider. Calculez une moyenne arithmétique ou une estimation au plus près, puis spécifiez le résultat pour chaque unité fonctionnelle. Utilisé pour les comptes état des résultats.| 
|Taux de fermeture | Utilisé pour les comptes de bilan.|
|Dernier taux de fermeture | Taux valide sur le marché des changes à la date pour laquelle le bilan ou l'état des résultats est préparé. Entrez ce taux pour chaque unité fonctionnelle. Utilisé pour les comptes de bilan.|
|Taux historique | Taux de change valide au moment de la transaction.|
|Taux composite | Les montants de la période en cours sont convertis au taux moyen et ajoutés au solde précédemment enregistré dans la compagnie consolidée. Cette méthode est généralement utilisée pour les comptes bénéfices non répartis, car ils incluent des montants provenant de périodes différentes et constituent donc un composé des montants convertis avec différents taux de change.|
|Taux des fonds propres | Il est similaire au **Taux composite**. Les différences sont reportées sur des comptes GL distincts.|   

Pour spécifier des taux de change pour les unités fonctionnelles, procédez comme suit :

1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Unités fonctionnelles**, puis sélectionnez le lien associé.  
2. Sur la page **Liste des unités fonctionnelles**, choisissez l'unité fonctionnelle, puis choisissez l'action **Taux moyen (manuel)**.   
3. Sur la page **Modifier taux de change**, la valeur du champ **Montant taux de change lié** est copiée à partir de la table **Taux de change devise**, mais vous pouvez la modifier. Fermez la page.  
4. Sous l'onglet **Naviguer**, dans le groupe **Taux change**, choisissez **Taux de clôture**.  
5. Dans le champ **Montant taux de change lié**, saisissez le taux de change. 

<!-- ### To include or exclude dimensions

COMMENTING THIS OUT BECAUSE i CANNOT REPRODUCE THE SETTINGS. tHERE IS NO CONSOLIDATION CODE FIELD ON DIMENSIONS OR DIMENSIOIN VALUES.

You can consolidate dimension information and general ledger accounts, as follows:

* To exclude dimension information in the consolidation, leave the **Consolidation Code** field blank, and do not choose dimensions in the **Copy Dimensions** fields in any consolidation functions or reports described later in this topic.
* To include dimension information in the consolidation, leave the **Consolidation Code** field blank. However, the consolidation will only work if the dimension values in the business unit are the same as the consolidated company.
* To consolidate the dimension value code in the business unit with a different dimension value code in the consolidated company, fill in the **Consolidation Code**. -->

### <a name="to-exclude-a-company-from-consolidation"></a>Pour exclure une compagnie de la consolidation
Si vous ne souhaitez pas inclure une unité fonctionnelle dans la consolidation, vous pouvez l'exclure. Pour ce faire, accédez à la fiche unité fonctionnelle et désactivez la case à cocher **Consolider**.

### <a name="to-include-a-partially-owned-company-in-consolidation"></a>Pour inclure une compagnie partiellement détenue dans la consolidation
Si vous détenez une compagnie en partie, vous pouvez ajouter un pourcentage de chaque transaction qui correspond au pourcentage de la compagnie que vous détenez. Par exemple, si vous possédez 70 % de la compagnie, la consolidation inclut 70 $ d'une facture de 100 $. Pour spécifier le pourcentage de la compagnie que vous détenez, accédez à la fiche unité fonctionnelle et saisissez le pourcentage dans le champ **% consolidation**.  

### <a name="to-test-the-data-before-you-consolidate"></a>Pour tester les données avant la consolidation
Vous pouvez tester vos données avant de les transférer vers la compagnie consolidée. [!INCLUDE[d365fin](includes/d365fin_md.md)] recherche des différences dans les informations des unités fonctionnelles et de la compagnie consolidée. Par exemple, si les numéros de compte ou les codes axe sont différents. Vous devez corriger les erreurs avant d'exécuter le rapport. Vous pouvez tester la base de données ou, si vous importez des données à partir d'un fichier XML, vous pouvez tester le fichier.   
  
1. Ouvrez la compagnie consolidée.  
2. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Unités fonctionnelles**, puis sélectionnez le lien associé.  
3. Exécutez l'une des opérations suivantes :  
  
    * Pour tester un fichier, choisissez l'action **Tester fichier**, entrez le nom du fichier à tester, puis choisissez **Imprimer**.  
    * Pour tester la base de données, choisissez **Tester base de données**.  

## <a name="to-run-the-consolidation"></a>Pour exécuter la consolidation
Une fois les données testées, vous pouvez les transférer vers la compagnie consolidée.  
  
1. Connectez-vous à la compagnie consolidée.  
2. Dans le **Tableau de bord Comptable**, choisissez l'action **Exécuter la consolidation**.  
3. Renseignez les champs requis.  
4. Dans le champ **Où**, choisissez **Nom de la compagnie**, puis choisissez la compagnie consolidée dans le champ **est**.  

## <a name="to-export-data-from-dynamics-nav-and-import-it-in-included365finincludesd365finmdmd"></a>Pour exporter des données depuis Dynamics NAV et les importer dans [!INCLUDE[d365fin](includes/d365fin_md.md)]
Si les données d'une unité fonctionnelle se trouvent dans une autre base de données, vous devez exporter les données dans un fichier avant de les inclure dans la consolidation. Chaque compagnie doit être exportée séparément. À cette fin, utilisez le traitement par lots **Exporter fichier consolidation**.  
  
Après l'exécution du traitement en lot, toutes les écritures des comptes GL sont traitées. Pour chaque combinaison d'axe principal et date sélectionnés, la valeur des champs **Montant** des écritures est totalisée et exportée. La combinaison d'axe principal et date sélectionnés suivante qui a le même numéro de compte est traitée, puis les combinaisons ayant le numéro de compte suivant sont traitées, etc.  

Les écritures exportées contiennent les champs suivants : **N° compte**, **Date comptabilisation** et **Montant**. Si des informations de dimensions ont également été exportées, des codes de dimension et des valeurs de dimension sont également inclus.  

1. Pour chaque ligne exportée, si le total des champs **Montant** est un débit, le numéro de compte configuré dans le champ **Compte débit consolidation** de l'unité fonctionnelle est exporté vers la ligne. Si le total est un crédit, le numéro correspondant dans le champ **Compte crédit consolidation** est exporté vers la ligne.  
2. La date utilisée pour chaque ligne exportée est la date de fin de la période ou, si le transfert est opéré chaque jour, la date du calcul.  
3. La section analytique exportée pour la saisie est celle de la société consolidée configurée dans le champ **Code consolidation** pour cette section analytique. Si aucune section analytique de société consolidée n'a été entrée dans le champ **Code consolidé** à cette fin, la section analytique proprement dite est exportée vers la ligne.   
4. Les fichiers XML contiennent également les taux de change devise correspondant à la période de consolidation. Ces taux sont inclus dans une section distincte au début du fichier.

## <a name="see-also"></a>Voir aussi
[Utilisation de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Exportation de vos données métier vers Excel](about-export-data.md)

