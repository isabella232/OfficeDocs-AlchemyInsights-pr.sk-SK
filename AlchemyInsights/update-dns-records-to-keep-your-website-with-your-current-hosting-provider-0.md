---
title: Aktualizácia záznamov DNS na ponechaie webovej lokality u aktuálneho poskytovateľa hostiteľských služieb
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827549"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="f6940-102">Aktualizácia záznamov DNS na ponechaie webovej lokality u aktuálneho poskytovateľa hostiteľských služieb</span><span class="sxs-lookup"><span data-stu-id="f6940-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="f6940-103">V Centre spravovania služby Microsoft 365 prejdite na stránku **Setup** Domains (Nastavenie domén) a v zozname domén vyberte doménu, ktorú používate pre  >  [](https://admin.microsoft.com/Adminportal#/Domains) svoju webovú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="f6940-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="f6940-104">Vyberte **položku + Nový vlastný záznam** a zadajte nasledovné položky:</span><span class="sxs-lookup"><span data-stu-id="f6940-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="f6940-105">Pre **typ DNS** zadajte: A **(Adresa)**</span><span class="sxs-lookup"><span data-stu-id="f6940-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="f6940-106">Do **poľa Názov hostiteľa alebo alias** zadajte nasledujúci reťazec: **@**</span><span class="sxs-lookup"><span data-stu-id="f6940-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="f6940-107">V **časti Adresa IP** zadajte statickú IP adresu svojej webovej lokality, na ktorej je momentálne hosťovaná (napríklad 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="f6940-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="f6940-108">Musí to byť  *statická*  IP adresa webovej lokality, nie  *dynamická*  IP adresa.</span><span class="sxs-lookup"><span data-stu-id="f6940-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="f6940-109">Overte lokalitu, na ktorej je hosťovaná vaša webová lokalita, a uistite sa, že môžete získať statickú IP adresu pre svoju verejnú webovú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="f6940-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="f6940-110">Vyberte **položku Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="f6940-110">Select **Save**.</span></span>

<span data-ttu-id="f6940-111">Okrem toho môžete vytvoriť záznam CNAME, ktorý zákazníkom pomôže nájsť vašu webovú lokalitu.</span><span class="sxs-lookup"><span data-stu-id="f6940-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="f6940-112">Vyberte **položku + Nový vlastný záznam** a zadajte nasledovné položky:</span><span class="sxs-lookup"><span data-stu-id="f6940-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="f6940-113">Pre **položku Typ DNS** zadajte: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="f6940-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="f6940-114">Do **poľa Názov hostiteľa alebo alias** zadajte: **www**</span><span class="sxs-lookup"><span data-stu-id="f6940-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="f6940-115">Do **poľa Points to address**(Body na adresu) zadajte plne kvalifikovaný názov domény (FQDN) svojej webovej lokality (napríklad contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f6940-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="f6940-116">Vyberte **položku Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="f6940-116">Select **Save**.</span></span>
