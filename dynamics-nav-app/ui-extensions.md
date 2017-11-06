---
title: Installer des extensions pour personnaliser Dynamics NAV
description: "En savoir plus sur l'ajout des fonctionnalit�s et la personnalisation de Dynamics NAV en installant des extensions."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: app, add-in, manifest, customize
ms.date: 07/07/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 109eb8d0e2a38566739878ef513ffa3bec8dcd30
ms.contentlocale: fr-ca
ms.lasthandoff: 10/26/2017

---
# <a name="customizing-dynamics-nav-using-extensions"></a>Personnalisation de Dynamics NAV � l'aide des extensions
Vous pouvez modifier [!INCLUDE[d365fin](includes/d365fin_md.md)] en installant des extensions qui ajoutent des fonctionnalit�s, modifient le comportement de l'application, ou vous permettent d'acc�der � de nouveaux services en ligne, par exemple.
La premi�re fois que vous lancez [!INCLUDE[d365fin](includes/d365fin_md.md)], certaines extensions sont d�j� install�es. Au fil du temps, davantage d'extensions seront disponibles. Il vous appartient de choisir si vous souhaitez les utiliser ou non.

Par exemple, Microsoft propose une extension qui fournit une int�gration � PayPal Payments Standard. Cette extension est install�e par d�faut.
Si une autre extension proposant une int�gration � un autre service de paiement devenait disponible, vous pouvez installer cette nouvelle extension et choisir lequel des deux services vous souhaitez utiliser.  

La fen�tre **Gestion des extensions** vous permet de g�rer les extensions. Vous pouvez acc�der � cette fen�tre � partir de la page d'accueil. Sinon, s�lectionnez l'ic�ne **Page ou �tat pour la recherche** ![Page ou �tat pour la recherche](media/ui-search/search_small.png "Ic�ne Page ou �tat pour la recherche") dans le coin sup�rieur droit, entrez **Extension**, puis s�lectionnez le lien associ�.  

> [!NOTE]  
>   Si vous voulez acc�der � une extension mais que vous ne pouvez pas trouver sa fonctionnalit�, v�rifiez la fen�tre **Gestion des extensions**, si l'extension n'est pas r�pertori�e, vous pouvez la configurer comme d�crit dans la section suivante.  

## <a name="installing-an-extension"></a>Installation d'une extension
Vous pouvez obtenir de nouvelles extensions depuis le march� � l'adresse [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1). Ici, vous trouverez toutes les extensions disponibles pour [!INCLUDE[d365fin](includes/d365fin_md.md)], et vous pourrez obtenir des applications, des extensions et des packs de contenu pour d'autres produits Microsoft. D�finissez les filtres appropri�s, observez les informations pour chaque extension et obtenez une extension pour votre [!INCLUDE[d365fin](includes/d365fin_md.md)].  
> [!NOTE]  
>   Connectez-vous au site [AppSource.microsoft.com](https://appsource.microsoft.com/) � l'aide du compte de messagerie �lectronique que vous utilisez pour [!INCLUDE[d365fin](includes/d365fin_md.md)]. Utilisez le m�me compte de messagerie �lectronique pour d'autres services et produits pour une exp�rience agr�able.  

Vous pouvez �galement acc�der au march� � partir de [!INCLUDE[d365fin](includes/d365fin_md.md)]. Dans la fen�tre **Gestion des extensions**, vous pouvez voir les extensions actuellement install�es, et vous pouvez ouvrir la page **March� des extensions** qui affiche les extensions [!INCLUDE[d365fin](includes/d365fin_md.md)] actuellement disponibles dans AppSource. Si vous optez pour le lien *Plus d'applications*, vous �tes dirig� vers le site [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).  

Si vous choisissez une extension, vous pouvez consulter une documentation relative � ses fonctionnalit�s, et acc�der au service d'aide de l'extension pour en savoir plus. Lorsque vous choisissez d'obtenir une extension, vous devez �tre d'accord avec les conditions d'utilisation. Si vous obtenez l'extension � partir du site Web AppSource, vous serez connect� � [!INCLUDE[d365fin](includes/d365fin_md.md)] pour terminer l'installation.  

Lorsque vous installez une extension, vous pouvez �tre amen� � la configurer, par exemple sp�cifier un compte � utiliser avec l'extension **PayPal Payments Standard pour [!INCLUDE[d365fin](includes/d365fin_md.md)]**.
D'autres extensions ajoutent simplement des champs � une page existante, ou ajoutent une nouvelle page, par exemple.   

Si vous d�sinstallez une extension, et que vous changez ensuite d'avis, vous pouvez la r�installer. Lorsque vous d�sinstallez une extension que vous avez utilis�, les donn�es sont conserv�es de sorte � demeurer disponibles si vous installez � nouveau l'extension.  

Certaines extensions sont fournies par Microsoft, et d'autres sont fournies par [d'autres soci�t�s](ui-extensions-other.md). Toutes les sont extensions test�es avant d'�tre mises � votre disposition, mais nous vous recommandons d'acc�der aux liens qui sont inclus dans chaque extension pour en savoir plus sur l'extension avant de d�cider de l'installer.  

Microsoft fournit les extensions suivantes�:  

* [Extension Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md)  
* [PayPal Payments Standard](ui-extensions-paypal-payments-standard.md)  
* [Extension QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md)  
* [Pr�vision des ventes et de l'inventaire](ui-extensions-sales-forecast.md)  
* [Extension Ceridian Payroll](ui-extensions-ceridian-payroll.md)  
* [Extension Importer le fichier de paie de Quickbooks](ui-extensions-quickbooks-payroll.md)  
* [Extension WorldPay Payments Standard](ui-extensions-worldpay-payments-standard.md)
* [Extension GetAddress.io UK Postcodes](ui-extensions-getaddressio.md)
* [Extension QuickBooks Online Data Migration](ui-extensions-quickbooks-online-data-migration.md)
* [Portail Comptable](ui-extensions-accountant-portal.md)  
* [Analyseur Image](ui-extensions-image-analyzer.md)

> [!NOTE]  
>  Les nouvelles extensions ne sont pas disponibles dans AppSource juste apr�s l'annonce d'une mise � jour. Vous pouvez vous tenir inform� sur les extensions sur le site [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).

## <a name="see-also"></a>Voir aussi
[Proc�dure�: activer les paiements client via Paypal](sales-how-enable-payment-service-extensions.md)  
[Migrer des donn�es m�tier � partir d'autres syst�mes financiers](upload-data.md)    
[Extensions [!INCLUDE[d365fin](includes/d365fin_md.md)] par d'autres fournisseurs](ui-extensions-other.md)  
[Bienvenue dans [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  

##


