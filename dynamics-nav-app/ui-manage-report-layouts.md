---
title: "Gérer des présentations de rapport"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 57cd575c1f72841dae162b077d1f676720ee24e7
ms.contentlocale: fr-ca
ms.lasthandoff: 06/26/2017

---
    
# <a name="manage-report-layouts"></a>Gérer des présentations de rapport
Une présentation de rapport contrôle le contenu et le format du rapport, dont les champs de données d'un ensemble de données de rapport apparaissant sur le rapport et la façon ils sont organisés, le style de texte, les images, et plus encore. À partir des clients Dynamics NAV, vous pouvez modifier la présentation utilisée pour un rapport, créer une présentation ou modifier les présentations existantes. 

En particulier, une présentation de rapport configure ce qui suit :

- Les champs d'étiquette et de données à inclure à partir de l'ensemble des données du rapport Dynamics NAV.
- Le format du texte, comme le type, la taille et la couleur de police.
- Le logo de la compagnie et son emplacement.
- Paramètres de page généraux, comme les marges et les images d'arrière-plan. 

Une instance Dynamics NAV peut être configurée avec plusieurs présentations de rapport. Vous pouvez ensuite passer de l'une à l'autre en fonction de vos besoins. Vous pouvez utiliser l'une des présentations de rapport intégrées ou vous pouvez créer des présentations de rapport personnalisées et les affecter à vos rapports selon vos besoins.

Vous pouvez utiliser deux types de présentations de rapport : Word et RDLC.

## <a name="word-report-layout-overview"></a>Aperçu de la présentation de rapport Word
Une présentation de rapport Word est basé sur un document Word (type de fichier .docx). Les présentations de rapport Word vous permettent de concevoir des présentations de rapport à l'aide de Microsoft Word 2013 ou une version ultérieure. Une présentation de rapport Word détermine le contenu du rapport, contrôle la manière dont les éléments de contenu sont organisés ainsi que leur apparence. Un document de présentation de rapport Word utilisera généralement des tableaux pour organiser le contenu, dans lequel les cellules peuvent contenir des champs de données, du texte ou des images.

## <a name="rdlc-layout-overview"></a>Aperçu de la présentation RDLC
Les présentations RDLC sont basées sur les présentations de définition de rapport client (types de fichier .rdlc or .rdl). Ces présentations sont créées et modifiées à l'aide du Générateur de rapports SQL Server. Le concept des présentations RDLC est similaire à celui des présentations Word, où la présentation définit le format général du rapport et détermine les champs de l'ensemble de données à inclure. La création de présentations RDLC est plus avancée que les présentations Word.

## <a name="built-in-and-custom-report-layouts"></a>Présentations de rapport intégrées et personnalisées
Dynamics NAV inclut plusieurs présentations intégrées. Les présentations intégrées sont des présentations prédéfinies conçues pour des états spécifiques. Les rapports Dynamics NAV comportent une présentation intégrée, RDLC, Word et parfois les deux. Il n'est pas possible de modifier une présentation de rapport intégrée à Dynamics NAV, mais vous pouvez l'utiliser comme point de départ pour créer vos propres présentations de rapport personnalisées. 

Les présentations personnalisées sont des présentations de rapport que vous créez pour modifier l'apparence d'un rapport. Vous créez généralement une présentation personnalisée basée sur une présentation intégrée, mais vous pouvez les créer de A à Z ou à partir d'une copie d'une présentation personnalisée existante. Les présentations personnalisées vous permettent d'avoir plusieurs présentations pour le même rapport, que vous choisissez en fonction de vos besoins. Par exemple, vous pouvez disposer de différentes présentations pour chaque compagnie Dynamics NAV, ou de plusieurs présentations pour la même compagnie pour des occasions ou événements spécifiques, comme une promotion spéciale ou la période des fêtes.

## <a name="deciding-whether-to-use-a-word-or-rdlc-report-layout"></a>Décider d'utiliser une présentation de rapport Word ou RDLC 
Une présentation de rapport peut être basée sur un document Word ou un fichier RDLC. Le choix entre une présentation de rapport Word ou une présentation de rapport RDLC dépendra de la façon dont vous souhaitez que le rapport généré apparaisse et de vos connaissances sur Word et SQL Server Report Builder. 

Les concepts généraux pour les présentations Word et RDLC sont très similaires. Cependant, la conception de chaque type présente certaines fonctionnalités qui affectent la manière dont le rapport généré s'affiche dans Dynamics NAV. Cela signifie que le même rapport peut sembler différent selon que vous utilisez une présentation de rapport Word ou une présentation de rapport RDLC.

Le procédure pour paramétrer des présentations de rapport Word et des présentations de rapport RDLC sur les rapports est la même. La principale différence réside dans la manière dont vous modifiez les présentations. Il est souvent plus facile de créer et de modifier des présentations de rapport Word que des présentations de rapport RDLC car vous pouvez utiliser Word. Les présentations de rapport RDLC sont modifiées à l'aide de SQL Server Report builder qui cible plus d'utilisateurs avancés.

Pour plus d'informations sur la manière d'utiliser l'une ou l'autre présentation, reportez-vous à [Procédure : modifiier la présentation actuellement utilisée sur un état](ui-how-change-layout-currently-used-report.md)

## <a name="see-also"></a>Voir aussi
[Utiliser Dynamics NAV](ui-work-product.md)  
[Procédure : Créer une présentation de rapport personnalisée](ui-how-create-custom-report-layout.md)  
[Procédure : envoyer des documents par e-mail](ui-how-send-documents-email.md)

