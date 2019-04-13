---
title: 1065 odsudzovanie EOP odchádzajúce IP adresa rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858111"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="d55fe-102">Odmietanie EOP odchádzajúce rozsahy adries IP</span><span class="sxs-lookup"><span data-stu-id="d55fe-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="d55fe-103">Zistili sme potenciálny problém s vašou organizáciou (ak nie je opravené 26 októbra 2018) by mohol zlomiť tok pošty lokálne alebo externé ciele.</span><span class="sxs-lookup"><span data-stu-id="d55fe-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="d55fe-104">Ako predtým oznámené, zjednodušiť spravovanie rozsah IP adries, sme sa konsolidácia rozsahy adries IP Exchange Online Protection (EOP), ktoré sa používajú na odosielať a prijímať e-maily mimo Office 365.</span><span class="sxs-lookup"><span data-stu-id="d55fe-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="d55fe-105">Naša analýza naznačuje, že jeden alebo viac zdrojov externých e-mailov alebo ciele, ktoré ste nakonfigurovali v pošty tok konektory nie sú prijímať pripojenia z IP adresy rozsahy uvedené [tu](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="d55fe-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="d55fe-106">Konať pred 26.októbra na zabezpečenie týchto zdrojov a destinácií bude akceptovať spojenie na všetky [uverejnené EOP IP adresy](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="d55fe-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="d55fe-107">Ďalšie informácie o tejto zmene nájdete Message Center príspevky [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)alebo [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="d55fe-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="d55fe-108">**Poznámka**: Ak ste predtým používali IP alebo adresu URL publikovanie cez HTML, XML a RSS aktualizácií endpoint, tiež by mali migrovať na nové webové služby pre automatizáciu týchto typov aktualizácií.</span><span class="sxs-lookup"><span data-stu-id="d55fe-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="d55fe-109">Ďalšie informácie nájdete v [kategórií koncový bod Office 365 a Office 365 IP adresa a adresa URL webovej služby](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="d55fe-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
