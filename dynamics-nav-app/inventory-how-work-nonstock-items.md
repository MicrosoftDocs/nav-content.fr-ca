---
title: "Procédure : utiliser des articles non stockés"
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 6d99e06c167d3b86db97883c02c8bf5cd746ae10
ms.contentlocale: fr-ca
ms.lasthandoff: 07/19/2017

---

# Procédure : utiliser des articles non stockés
Vous pouvez proposer certains articles à vos clients pour leur rendre service, que vous ne souhaitez pas conserver dans l'inventaire tant que vous ne commencez pas à les commercialiser. Lorsque vous souhaitez commencer à stocker ces articles dans l'inventaire, vous pouvez les convertir en fiches article normales de deux façons.

- Depuis une fiche article non stocké, créez une nouvelle fiche article basée sur un modèle.
- Depuis une ligne commande vente avec un champ **Article** vide, sélectionnez un article non stocké. Lorsque vous reportez la vente, une fiche article est automatiquement créée pour l'article non stocké.

**Remarque** : vous ne pouvez pas sélectionner d'article non stocké à partir de la fenêtre **Facture vente**. Vous pouvez sélectionner un article non stocké à partir de la fenêtre **Devis**, mais l'article non stocké ne sera pas converti en un article normal lorsque vous utilisez la fonction **Créer commande**.

Un article non stocké a généralement le numéro d'article du fournisseur qui le fournit. Pour activer la conversion d'une fiche article non stocké en une fiche article normale, vous devez tout d'abord configurer comment la numérotation de l'article fournisseur est convertie dans votre propre numérotation d'article.   

## Pour créer un article non stocké
Les fiches article non stocké ont moins d'informations que les fiches article normales, car vous ne les utilisez que pour proposer des devis ainsi que pour d'autres procédures. Pour cette raison, elles doivent être converties en fiches article normales, avant que vous puissiez reporter les transactions commerciales pour elles.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Articles non stockés**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau**.
2. Renseignez les champs selon vos besoins. Choisissez un champ pour lire une brève description du champ ou du lien vers plus d'informations.

## Pour configurer comment les numéros d'article non stocké sont convertis en votre propre numérotation  
Pour activer la conversion d'une fiche article non stocké en une fiche article normale, vous devez tout d'abord configurer comment la numérotation de l'article fournisseur est convertie dans votre propre format de numérotation d'article.

1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Paramètres art. non stockés**, puis sélectionnez le lien connexe.
2. Renseignez les champs selon vos besoins.

## Pour convertir un article non stocké en un article normal
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Articles non stockés**, puis sélectionnez le lien connexe.
2. Ouvrez la fiche pour un article non stocké que vous pouvez convertir en un article normal.
3. Dans la fenêtre **Fiche article non stocké**, sélectionnez l'action **Créer un article**.

Une nouvelle fiche article pré-remplie avec les informations de l'article non stocké ainsi qu'un modèle d'article pertinent sont créés. Vous pouvez ensuite remplir ou modifier les champs sur la nouvelle fiche article, le cas échéant. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux produits](inventory-how-register-new-products.md).

## Pour vendre un article non stocké et le convertir en article normal
1. Dans le coin supérieur droit, sélectionnez l'icône **Page ou état pour la recherche**, saisissez **Commandes vente**, puis sélectionnez le lien connexe.
2. Sélectionnez l'action **Nouveau**. complétez les champs du raccourci **Général** comme pour toute commande vente.
3. Sur une nouvelle ligne vente, laissez le champ **Article** vide, sélectionnez **Ligne**, **Fonctions**, puis sélectionnez **Articles non stockés**.

    L'article non stocké est converti en un article normal. Une nouvelle fiche article pré-remplie avec les informations de l'article non stocké ainsi qu'un modèle d'article pertinent sont créés.
4. Dans la fenêtre **Articles non stockés**, sélectionnez l'article non stocké que vous souhaitez vendre, puis choisissez le bouton **OK**.
5. Lorsque les lignes commande vente sont renseignées, sélectionnez l'action **Valider**.

Vous pouvez ensuite remplir ou modifier les champs sur la nouvelle fiche article, le cas échéant. Pour plus d'informations, reportez vous à [Procédure : enregistrer de nouveaux produits](inventory-how-register-new-products.md).

**Remarque** : un enregistrement de référence externe article est automatiquement créé pour le fournisseur de l'article entre le numéro article fournisseur et votre nouveau numéro article.

## Voir aussi
[Procédure : enregistrer de nouveaux produits](inventory-how-register-new-products.md)  
[Gestion du stock](inventory-manage-inventory.md)  
[Utiliser Dynamics NAV](ui-work-product.md)

