---
title: "Procédure : créer des commandes service"
description: "Utilisez la fenêtre **Commande service** pour créer des documents dans lesquels vous saisissez des informations sur un service, tel que les réparations et l'entretien, pour des articles de service à la demande du client."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: aa0578c7311fcd997653c6dc6d31325abd1d367c
ms.contentlocale: fr-ca
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-service-orders"></a>Procédure : créer des commandes service
Utilisez la fenêtre **Commande service** pour créer des documents dans lesquels vous saisissez des informations sur un service, tel que réparation et maintenance, pour des articles de service à la demande du client.  
  
Lorsque vous créez une commande service, vous ne devez renseigner que certains champs. Certains champs sont facultatifs et la beaucoup d'entre eux sont renseignés automatiquement lorsque vous renseignez les champs associés.  
  
## <a name="to-create-a-service-order"></a>Pour créer une commande service    
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Commandes de service**, puis sélectionnez le lien associé.  
2. Créez une nouvelle commande service.  
3. Dans le champ **N°**, saisissez le numéro de la commande service.  
  
     Si vous avez configuré une souche de numéros pour les commandes de service dans la fenêtre **Paramètres Gestion des services,** vous pouvez appuyer sur Entrée pour renseigner le numéro de commande service suivant.  
  
4. Dans le champ **N° client**, sélectionnez le client approprié dans la liste. Les champs client pertinents sont automatiquement renseignés avec les informations de la table **Client**.  
  
5. Selon les paramètres du raccourci **Champs obligatoires** de la fenêtre **Config. gestion des services**, vous pouvez être amené à renseigner le champ **Type commande service** et le champ **Code représentant**.  
6. De manière optionnelle, renseignez les autres champs.  
7. Enregistrez les lignes article de service.  

## <a name="to-create-a-service-order-from-a-contract"></a>Pour créer une commande de service à partir d'un contrat  
Vous pouvez créer automatiquement des commandes service pour l'entretien des articles de service sur la base des contrats de service.  
  
1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Créer des commandes de service de contrat**, puis sélectionnez le lien associé.  
2. Sur le raccourci **En-tête contrat service**, positionnez les filtres à appliquer.  
3. Sur le raccourci **Options** , renseignez les champs **Date début** et **Date fin** avec la date début et la date fin pour la période pour laquelle vous souhaitez créer les commandes contrat de service. Le traitement en lot crée des commandes service qui incluent les articles de service des contrats de service dont les dates service suivantes sont comprises dans cette période.  
  
    > [!NOTE]  
    >  Le nombre de jours que vous pouvez utiliser comme plage de dates à chaque utilisation de ce traitement en lot est limité. Vous définissez cette limite dans le champ **Nbre jours max. cde contrat** de la fenêtre **Paramètres Gestion des services**.  
  
4. Dans le champ **Action**, sélectionnez **Créer commande service**.  

## <a name="to-convert-a-service-quote-to-a-service-order"></a>Pour convertir les devis service en commandes service
Lorsqu'un client accepte un devis service, vous le convertissez en commande service. Le devis est effacé et une commande service avec la même description que le devis service est crée. La date et le délai de réponse de la commande service sont recalculés et est affecté à cette dernière le statut **Suspendu**. L'état réparation des articles de service de la commande est modifié en **Initial**.  
  
[!INCLUDE[d365fin](includes/d365fin_md.md)] recherche les écritures affectation de tous les articles de service du devis service qui présentent le statut **Actif**. S'il en trouve, leur état d'affectation passe à **Réaffectation nécessaire**. Lorsque vous réaffectez les articles de service de la commande service, le statut des écritures affectation enregistrées pour le devis passe à **Terminé**.   

1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Devis de contrat de service**, puis sélectionnez le lien associé.  
2. Choisissez le devis service à convertir en commande service.  
3. Sélectionnez l'action **Créer commande**.  

## <a name="to-check-item-availability-for-one-or-more-orders"></a>Pour vérifier la disponibilité des articles pour une ou plusieurs commandes  
Vous pouvez vérifier si un article dont vous avez besoin pour une commande est en stock et, s'il ne l'est pas, la date à laquelle il le sera. En outre, si un article est disponible à la réservation, vous pouvez le réserver pour vous assurer qu'il sera disponible. Vous pouvez vérifier la disponibilité pour une commande définie, ou pour toutes les commandes.  

1.  Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Tableau d'affectation**, puis sélectionnez le lien associé.  
2. Exécutez l'une des opérations suivantes :  
  
    * Pour une commande définie, choisissez la commande, puis sélectionnez l'action **Aperçu demande**.  
    * Pour toutes les commandes, choisissez **Afficher document**. La fenêtre **Commande service** s'ouvre.  
  
3. Sur la page **Aperçu demande**, développez le regroupement d'articles et afficher des informations sur la disponibilité de l'article. Par exemple, vous pouvez visualiser le nombre d'articles en inventaire. Vous pouvez également consulter si l'article d'une commande en attente est disponible, c'est-à-dire Type origine = achat, ou la date à laquelle il le sera ou s'il a été réservé. 

## <a name="to-reserve-an-item-for-a-service-order"></a>Pour réserver un article pour une commande service
Si vous voulez avoir l'assurance qu'un article est disponible pour une commande service, vous pouvez réserver l'article. 

1. Dans la zone **Rechercher**, entrez **Commandes service**, puis sélectionnez le lien associé.  
2. Cliquez sur la commande service, puis choisissez **Modifier**.  
3. Sélectionnez **Actions**, **Commande**, puis **Lignes service**.  
4. Sur la page **Lignes service**, sélectionnez l'article à réserver, puis sélectionnez l'action **Réserver**.  
5. Sur la page **Réservation**, choisissez **Réserver à partir de la ligne courante**. 

## <a name="to-insert-lines-based-on-standard-service-codes"></a>Pour insérer des lignes selon les codes prestation standard  
Si vous avez configuré des codes prestation standard et les avez associés à des groupes articles de service, vous pouvez insérer les lignes standard liées aux codes prestation standard sur des documents service. Pour plus d'informations, reportez vous à [Procédure : configurer des codes prestation standard](service-how-setup-service-coding.md).   

1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Commandes de service**, puis sélectionnez le lien associé.  
2. Créez une nouvelle commande service.  
3. Renseignez les champs selon vos besoins.  
4. Renseignez les lignes article de service avec les informations requises.  
5. Choisissez la ligne contenant l'article de service pour lequel vous souhaitez créer des lignes service, puis choisissez **Extraire codes prestation std**. La fenêtre **Codes gpe articles de service standard** s'affiche avec les codes standard pour le groupe articles de service spécifié sur la ligne.  
6. Choisissez le code approprié, puis choisissez le bouton **OK** pour entrer les lignes service standard.  
  
> [!NOTE]  
>  Si le champ **Code gpe articles de service** de la ligne article de service du document est vide, cela signifie que l'article de service n'appartient à aucun groupe articles de service. Dans ce cas, la fenêtre **Codes gpe articles de service standard** contient la liste de tous les codes prestation standard. Vous devez sélectionner dans la liste les lignes service standard à insérer dans le document. Vous pouvez également sélectionner dans la liste des codes prestation standard affectés à un groupe articles de service spécifique. Pour afficher la liste, sélectionnez le code approprié dans le champ **Code gpe articles de service** dans la fenêtre **Codes gpe articles de service standard**.  

## <a name="to-register-internal-or-public-comments"></a>Pour enregistrer des commentaires internes ou publics
Vous pouvez ajouter des commentaires qui sont imprimés sur les commandes service et devis service pour fournir des informations supplémentaires. Vous pouvez saisir un maximum de 80 caractères, espaces compris. Si vous souhaitez saisir un texte supplémentaire, choisissez une autre ligne. Pour enregistrer un commentaire, sélectionnez une ligne, puis choisissez l'action **Commentaires**.  

## <a name="to-delete-invoiced-service-orders"></a>Pour supprimer des commandes service facturées  
Les commandes sont habituellement supprimées automatiquement après avoir été entièrement facturées. Lors de la validation d'une facture, une écriture correspondante est générée dans la fenêtre **Factures service enreg.**. Vous pouvez afficher le document reporté sur la page **Facture de service reportée**.  
  
Le programme ne supprime pas la commande service automatiquement cependant, si la quantité totale sur la commande a été validée, non pas à partir de la commande service proprement dite, mais à partir de la fenêtre **Facture service**. Ensuite, il se peut que vous deviez supprimer des commandes facturées qui n'ont pas été supprimées. Pour ce faire, exécutez le traitement par lots **Supprimer commandes service facturées**.  

1. Choisissez l'icône ![Page ou rapport pour la recherche](media/ui-search/search_small.png "icône Page ou rapport pour la recherche"), entrez **Supprimer les commandes de service facturées**, puis sélectionnez le lien associé. La fenêtre de demande du traitement par lots **Supprimer commandes service facturées** s'ouvre.  
2. Pour sélectionner les commandes à supprimer, vous pouvez positionner des filtres dans les champs **N°**, **N° client** et **N° client facturé**. .  
3. Cliquez sur le bouton **OK**.  


## <a name="see-also"></a>Voir aussi  
[Validation de service](service-service-posting.md)  
[Procédure : reporter une commande service](service-how-to-post-service-orders.md)  
[Paramétrage de la gestion des services](service-setup-service.md)  
[Procédure : travailler sur des tâches service](service-how-to-work-on-service-tasks.md)  
[Procédure : affecter des ressources](service-how-to-allocate-resources.md)  

