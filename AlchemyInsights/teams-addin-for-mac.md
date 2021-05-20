---
title: Teams pre Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582085"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="ed159-102">Teams pre Mac</span><span class="sxs-lookup"><span data-stu-id="ed159-102">Teams add-in for Mac</span></span>

<span data-ttu-id="ed159-103">Ak chcete vyriešiť problém Teams používateľom chýbajúceho doplnku pre Mac, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="ed159-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="ed159-104">**Krok 1:** Ak máte hybridné Exchange lokálne (vyžaduje sa 2016 CU3 alebo novšia verzia), pomocou nástroja Test-HMA.ps1 overte, či je hybridné moderné overovanie správne nakonfigurované.</span><span class="sxs-lookup"><span data-stu-id="ed159-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="ed159-105">Ďalšie informácie nájdete v téme [Overenie nastavenia hybridného moderného overovania pre Outlook pre iOS a Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="ed159-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="ed159-106">**Poznámka** Použite formát adresy menom používateľa (napríklad username@contoso.com [),](mailto:username@contoso.com)nie doména\menopoužívateľa.</span><span class="sxs-lookup"><span data-stu-id="ed159-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="ed159-107">Tento to môžete urobiť aj pre používateľov s Exchange Online poštovou Exchange Online poštovou schránkami.</span><span class="sxs-lookup"><span data-stu-id="ed159-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="ed159-108">**Krok 2:** Uchyťte používateľa prejsť **na položku Kontá**  >  **nástrojov**... in Outlook pre Mac, and find and select the account.</span><span class="sxs-lookup"><span data-stu-id="ed159-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="ed159-109">Potvrďte, že meno používateľa je vo formáte uvedeného užívateľa [(napríklad username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="ed159-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="ed159-110">**Krok 3:** Potvrďte, že používateľ je licencovaný Microsoft Teams používateľa.</span><span class="sxs-lookup"><span data-stu-id="ed159-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="ed159-111">Používateľ musí používať predplatné na Office 365 pre Mac, verziu produktu 16.24 alebo novšiu.</span><span class="sxs-lookup"><span data-stu-id="ed159-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>