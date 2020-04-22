---
title: 1065 deaktivácia EOP odchádzajúce IP adresa rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704612"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="dad6a-102">Deprecácia rozsahov IP odchádzajúcich adries EOP</span><span class="sxs-lookup"><span data-stu-id="dad6a-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="dad6a-103">Zistili sme potenciálny problém s vašou organizáciou, že (ak nie je opravené 26. októbra, 2018) môže zlomiť tok pošty do lokálnych alebo externých destinácií.</span><span class="sxs-lookup"><span data-stu-id="dad6a-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="dad6a-104">Ako už bolo oznámené, zjednodušiť riadenie rozsahu adries IP, sme konsolidácia Exchange Online Protection (EOP) IP adries rozsahy, ktoré sa používajú na odosielanie a prijímanie e-mailov mimo Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dad6a-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="dad6a-105">Z našej analýzy vyplýva, že jeden alebo viac externých e-mailových zdrojov alebo cieľových miest, ktoré ste nakonfigurovali v konektoroch toku pošty, neprijímajú pripojenia z rozsahov adries IP, ktoré sú [tu](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)zobrazené.</span><span class="sxs-lookup"><span data-stu-id="dad6a-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="dad6a-106">Zákon pred 26. října na zabezpečenie týchto zdrojov a destinácií bude akceptovať pripojenie k a zo všetkých [publikovaných EOP IP adresy](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="dad6a-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="dad6a-107">Ďalšie informácie o tejto zmene nájdete centrum správ príspevky [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)alebo [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="dad6a-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="dad6a-108">**Poznámka**: Ak ste predtým používali IP alebo URL publikovanie prostredníctvom HTML, XML a RSS pre Endpoint aktualizácie, mali by ste tiež migrovať na nové webové služby pre automatizáciu týchto typov aktualizácií.</span><span class="sxs-lookup"><span data-stu-id="dad6a-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="dad6a-109">Ďalšie informácie nájdete v téme [microsoft 365 koncový bod kategórie a microsoft 365 adresu IP a URL webovej služby](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="dad6a-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
