---
title: OneDrive for Business web OneDrive presmeruje, aby sa ponorili
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
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776395"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="d3f07-102">Presmerované na preniknúť po kliknutí na položku OneDrive</span><span class="sxs-lookup"><span data-stu-id="d3f07-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="d3f07-103">Pozrite si podrobný [návod na riešenie problémov](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="d3f07-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="d3f07-104">Ak chcete tento problém vyriešiť, správca musí používateľovi udeliť právo na vytvorenie lokality osobnej lokality.</span><span class="sxs-lookup"><span data-stu-id="d3f07-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="d3f07-105">Je to preto, lebo na mojich lokalitách sa vytvorí stránka OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="d3f07-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="d3f07-106">Ak chcete udeliť toto právo, postupujte podľa týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="d3f07-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="d3f07-107">V centre spravovania služby SharePoint kliknite na položku **používateľské profily**.</span><span class="sxs-lookup"><span data-stu-id="d3f07-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="d3f07-108">V časti **ľudia** kliknite na položku **Spravovať povolenia používateľov**.</span><span class="sxs-lookup"><span data-stu-id="d3f07-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="d3f07-109">Pridajte používateľov, ktorí potrebujú povolenia na vytvorenie lokality osobnej lokality.</span><span class="sxs-lookup"><span data-stu-id="d3f07-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="d3f07-110">Toto nastavenie je predvolene nastavené na hodnotu **všetci okrem externých používateľov**.</span><span class="sxs-lookup"><span data-stu-id="d3f07-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="d3f07-111">Po pridaní používateľa, používateľov alebo skupiny Skontrolujte, či je vybratý pridaný používateľ, používatelia alebo skupina, posuňte sa na časť **povolenia** a potom začiarknite políčko vedľa položky **vytvoriť osobnú lokalitu (vyžadované pre osobný ukladací priestor, informačný kanál s aktualizáciami a sledovaný obsah)**.</span><span class="sxs-lookup"><span data-stu-id="d3f07-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="d3f07-112">Kliknite na **tlačidlo OK**a potom ho používateľ vyhľadá na stránku OneDrive a vytvorí lokalitu.</span><span class="sxs-lookup"><span data-stu-id="d3f07-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
