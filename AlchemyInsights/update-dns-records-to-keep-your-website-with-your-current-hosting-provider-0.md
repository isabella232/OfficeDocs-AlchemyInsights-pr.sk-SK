---
title: Aktualizácie záznamov DNS, aby vaše webové stránky s aktuálne poskytovateľa hostingu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665775"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="931c7-102">Aktualizácie záznamov DNS, aby vaše webové stránky s aktuálne poskytovateľa hostingu</span><span class="sxs-lookup"><span data-stu-id="931c7-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="931c7-103">Microsoft 365 admin Center, prejdite na **Nastavenie** > [domén](https://portal.office.com/adminportal/home#/Domains) strana a v zozname domény vyberte doménu, ktorú používate pre vaše webové stránky.</span><span class="sxs-lookup"><span data-stu-id="931c7-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="931c7-104">Vyberte položku **+ nový vlastný rekord** a zadajte nasledujúce:</span><span class="sxs-lookup"><span data-stu-id="931c7-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="931c7-105">Pre **Typ DNS** zadajte: **(adresa)**</span><span class="sxs-lookup"><span data-stu-id="931c7-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="931c7-106">Pre **názov hostiteľa alebo Alias**, zadajte nasledovný príkaz:**@**</span><span class="sxs-lookup"><span data-stu-id="931c7-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="931c7-107">**Adresa IP**zadajte statickú adresu IP pre vaše webové stránky, kde je v súčasnosti hostil (napríklad 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="931c7-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="931c7-108">Musí to byť *statická* adresa IP pre webové stránky, nie *dynamickú* IP adresu.</span><span class="sxs-lookup"><span data-stu-id="931c7-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="931c7-109">Skontrolujte s lokalitou, kde je hostiteľom vašich webových stránkach aby sa ubezpečil, môžete získať statickú adresu IP pre vaše verejné webové stránky.</span><span class="sxs-lookup"><span data-stu-id="931c7-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="931c7-110">Kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="931c7-110">Select **Save**.</span></span>

<span data-ttu-id="931c7-111">Okrem toho môžete vytvoriť záznam CNAME pre zákazníkov nájsť vaše webové stránky.</span><span class="sxs-lookup"><span data-stu-id="931c7-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="931c7-112">Vyberte položku **+ nový vlastný rekord** a zadajte nasledujúce:</span><span class="sxs-lookup"><span data-stu-id="931c7-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="931c7-113">Pre **Typ DNS** zadajte: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="931c7-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="931c7-114">Pre **názov hostiteľa alebo Alias**, zadajte nasledujúce: **www**</span><span class="sxs-lookup"><span data-stu-id="931c7-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="931c7-115">**Bodov na adresu**, zadajte plne kvalifikovaní doménové meno (FQDN) pre vaše webové stránky (napríklad contoso.com).</span><span class="sxs-lookup"><span data-stu-id="931c7-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="931c7-116">Kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="931c7-116">Select **Save**.</span></span>
