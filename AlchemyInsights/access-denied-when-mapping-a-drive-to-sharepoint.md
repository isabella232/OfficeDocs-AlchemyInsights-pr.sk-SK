---
title: Prístup odmietnutý pri mapovaní jednotky na SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668758"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="7c9dd-102">Riešenie problémov s knižnicami SharePointu priradenými k sieťovým jednotkám</span><span class="sxs-lookup"><span data-stu-id="7c9dd-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="7c9dd-103">Pri prehľadávaní priradenej sieťovej jednotky sa môže zobraziť jedno z nasledujúcich hlásení:</span><span class="sxs-lookup"><span data-stu-id="7c9dd-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="7c9dd-104">**\\Cesta nie je prístupná. Pravdepodobne nemáte povolenie na používanie tohto sieťového zdroja. Ak chcete zistiť, či máte povolenia na prístup, obráťte sa na správcu tohto servera.**</span><span class="sxs-lookup"><span data-stu-id="7c9dd-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="7c9dd-105">**Prístup bol odmietnutý. Pred otvorením súborov v tomto umiestnení je najprv potrebné pridať webovú lokalitu do zoznamu dôveryhodných lokalít, prejsť na webovú lokalitu a vybrať možnosť automatického prihlásenia.**</span><span class="sxs-lookup"><span data-stu-id="7c9dd-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="7c9dd-106">[Získajte pomoc pri riešení problémov s priradenými sieťovými jednotkami](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="7c9dd-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="7c9dd-107">Mapovanie knižnice ako sieťovej jednotky je dočasné a podporované len v Internet Exploreri.</span><span class="sxs-lookup"><span data-stu-id="7c9dd-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="7c9dd-108">Namiesto toho [Synchronizujte súbory SharePointu s novým synchronizačným klientom pre OneDrive](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) , ktorý obsahuje [súbory na požiadanie](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="7c9dd-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="7c9dd-109">Pristupujte k všetkým súborom vo OneDrive bez použitia lokálneho ukladacieho priestoru.</span><span class="sxs-lookup"><span data-stu-id="7c9dd-109">Access all your files in OneDrive without using local storage space.</span></span>
  