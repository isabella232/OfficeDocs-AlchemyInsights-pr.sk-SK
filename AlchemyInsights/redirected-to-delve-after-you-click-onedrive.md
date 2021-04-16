---
title: OneDrive for Business Web OneDrive presmeruje do služby Delve
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
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51800004"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="8e5c2-102">Presmerované do Delve po kliknutí na položku OneDrive</span><span class="sxs-lookup"><span data-stu-id="8e5c2-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="8e5c2-103">Pozrite si našu podrobnú [príručku na riešenie problémov.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="8e5c2-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="8e5c2-104">Na vyriešenie tohto problému musí správca udeliť používateľom právo na vytvorenie svojej lokality moje lokality.</span><span class="sxs-lookup"><span data-stu-id="8e5c2-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="8e5c2-105">Je to spôsobené tým, že stránka služby OneDrive for Business sa vytvára na lokalite Moje lokality.</span><span class="sxs-lookup"><span data-stu-id="8e5c2-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="8e5c2-106">Ak chcete toto právo udeliť, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="8e5c2-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="8e5c2-107">V Centre spravovania služby SharePoint kliknite na položku **Používateľské profily**.</span><span class="sxs-lookup"><span data-stu-id="8e5c2-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="8e5c2-108">V časti **Ľudia** kliknite na položku **Spravovať povolenia používateľov**.</span><span class="sxs-lookup"><span data-stu-id="8e5c2-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="8e5c2-109">Pridajte používateľov, ktorí vyžadujú povolenia na vytvorenie ich lokality Moje lokality.</span><span class="sxs-lookup"><span data-stu-id="8e5c2-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="8e5c2-110">Predvolene je toto nastavenie nastavené na hodnotu Všetci **okrem externých používateľov.**</span><span class="sxs-lookup"><span data-stu-id="8e5c2-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="8e5c2-111">Po pridaní používateľa, používateľov alebo skupiny skontrolujte, či je vybratý pridaný používateľ, používatelia  alebo skupina, posuňte sa do sekcie povolení a potom začiarknite políčko vedľa položky Vytvoriť osobnú lokalitu (vyžaduje sa pre osobný ukladací priestor, kanál s aktualizáciami a sledovaný **obsah).**</span><span class="sxs-lookup"><span data-stu-id="8e5c2-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="8e5c2-112">Kliknite na tlačidlo **OK** a potom používateľ musí prejsť na stránku OneDrive a vytvoriť lokalitu.</span><span class="sxs-lookup"><span data-stu-id="8e5c2-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
