---
title: Aktualizácia DNS záznamov, aby sa vaša webová lokalita udržala u aktuálneho poskytovateľa hostiteľských služieb
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665775"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="31797-102">Aktualizácia DNS záznamov, aby sa vaša webová lokalita udržala u aktuálneho poskytovateľa hostiteľských služieb</span><span class="sxs-lookup"><span data-stu-id="31797-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="31797-103">V Centre spravovania služby Microsoft 365 prejdite na stránku **Setup**  >  [Domains (Nastavenia domén)](https://portal.office.com/adminportal/home#/Domains) a v zozname domén vyberte doménu, ktorú používate pre svoju webovú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="31797-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="31797-104">Vyberte **položku + Nový vlastný záznam** a zadajte nasledujúce položky:</span><span class="sxs-lookup"><span data-stu-id="31797-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="31797-105">Pre **typ DNS** zadajte: A **(Adresa)**</span><span class="sxs-lookup"><span data-stu-id="31797-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="31797-106">Pre **názov hostiteľa alebo alias**, zadajte nasledovné:**@**</span><span class="sxs-lookup"><span data-stu-id="31797-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="31797-107">V prípade **adresy IP**zadajte statickú adresu IP webovej lokality, na ktorej je aktuálne hosťovaná (napríklad 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="31797-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="31797-108">Musí to byť *statická* adresa IP pre webovú lokalitu, nie *dynamická* adresa IP.</span><span class="sxs-lookup"><span data-stu-id="31797-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="31797-109">Informujte sa u stránok, kde je vaša webová stránka hosťovaná, aby sa ubezpečil, môžete získať statickú IP adresu pre vaše verejné webové stránky.</span><span class="sxs-lookup"><span data-stu-id="31797-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="31797-110">Vyberte polo **ku Ulo3/4i»**.</span><span class="sxs-lookup"><span data-stu-id="31797-110">Select **Save**.</span></span>

<span data-ttu-id="31797-111">Okrem toho môžete vytvoriť CNAME záznam, ktorý pomôže zákazníkom nájsť vaše webové stránky.</span><span class="sxs-lookup"><span data-stu-id="31797-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="31797-112">Vyberte **položku + Nový vlastný záznam** a zadajte nasledujúce položky:</span><span class="sxs-lookup"><span data-stu-id="31797-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="31797-113">Pre **typ DNS** zadajte: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="31797-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="31797-114">Pre **názov hostiteľa alebo Alias**zadajte nasledujúce: **www**</span><span class="sxs-lookup"><span data-stu-id="31797-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="31797-115">Ak **chcete použiť položku Smerovanie na adresu,** zadajte úplný názov domény (FQDN) pre vašu webovú lokalitu (napríklad contoso.com).</span><span class="sxs-lookup"><span data-stu-id="31797-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="31797-116">Vyberte polo **ku Ulo3/4i»**.</span><span class="sxs-lookup"><span data-stu-id="31797-116">Select **Save**.</span></span>
