---
title: Aktualizujte DNS záznamy, aby ste mali webovú lokalitu so súčasným poskytovateľom hostiteľských služieb.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699534"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="0cbd2-102">Aktualizujte DNS záznamy, aby ste mali webovú lokalitu so súčasným poskytovateľom hostiteľských služieb.</span><span class="sxs-lookup"><span data-stu-id="0cbd2-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="0cbd2-103">V centre spravovania služby Microsoft 365 prejdite na stránku **Nastavenie**  >  [domén](https://portal.office.com/adminportal/home#/Domains) a v zozname domén vyberte doménu, ktorú používate pre svoju webovú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="0cbd2-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="0cbd2-104">Vyberte položku **+ nový vlastný záznam** a zadajte tieto možnosti:</span><span class="sxs-lookup"><span data-stu-id="0cbd2-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="0cbd2-105">**Typ DNS** zadajte: **A (adresa)**</span><span class="sxs-lookup"><span data-stu-id="0cbd2-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="0cbd2-106">Pre **názov hostiteľa alebo alias**zadajte nasledovné: **@**</span><span class="sxs-lookup"><span data-stu-id="0cbd2-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="0cbd2-107">Pre **adresu IP**zadajte statickú IP adresu svojej webovej lokality, na ktorej je v súčasnosti hosťovaná (napríklad 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="0cbd2-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="0cbd2-108">Musí to byť  *statická*  IP adresa webovej lokality, nie  *dynamická*  IP adresa.</span><span class="sxs-lookup"><span data-stu-id="0cbd2-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="0cbd2-109">Skontrolujte, či je lokalita, na ktorej je vaša webová lokalita hosťovaná, a uistite sa, že môžete získať statickú IP adresu svojej verejnej webovej lokality.</span><span class="sxs-lookup"><span data-stu-id="0cbd2-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="0cbd2-110">Vyberte položku **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="0cbd2-110">Select **Save**.</span></span>

<span data-ttu-id="0cbd2-111">Okrem toho môžete vytvoriť CNAME záznam, ktorý zákazníkom pomôže nájsť vašu webovú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="0cbd2-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="0cbd2-112">Vyberte položku **+ nový vlastný záznam** a zadajte tieto možnosti:</span><span class="sxs-lookup"><span data-stu-id="0cbd2-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="0cbd2-113">**Typ DNS** zadajte: **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="0cbd2-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="0cbd2-114">Ak máte **názov hostiteľa alebo alias**, zadajte: **www**</span><span class="sxs-lookup"><span data-stu-id="0cbd2-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="0cbd2-115">V prípade **bodov na adresu**Zadajte úplný názov domény (FQDN) svojej webovej lokality (napríklad contoso.com).</span><span class="sxs-lookup"><span data-stu-id="0cbd2-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="0cbd2-116">Vyberte položku **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="0cbd2-116">Select **Save**.</span></span>
