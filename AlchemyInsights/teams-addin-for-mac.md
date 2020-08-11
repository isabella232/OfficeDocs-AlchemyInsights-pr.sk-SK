---
title: Doplnok teams pre Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629883"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="31512-102">Doplnok teams pre Mac</span><span class="sxs-lookup"><span data-stu-id="31512-102">Teams add-in for Mac</span></span>

<span data-ttu-id="31512-103">Ak chcete vyriešiť problém s chýbajúcimi tímami pre používateľov operačných systémov pre Mac, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="31512-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="31512-104">**Krok 1:** Ak máte lokálne hybridné Exchange (2016 CU3 alebo novšiu verziu), pomocou nástroja Test-HMA.ps1 potvrďte, že hybridné moderné overovanie je správne nakonfigurované.</span><span class="sxs-lookup"><span data-stu-id="31512-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="31512-105">Ďalšie informácie nájdete v téme [overovanie hybridného moderného nastavenia overovania pre Outlook pre iOS a Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="31512-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="31512-106">**Poznámka:** Použite formát adresy UPN (napríklad [username@contoso.com](mailto:username@contoso.com)), nie Domain\Username.</span><span class="sxs-lookup"><span data-stu-id="31512-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="31512-107">Urobte to aj pre používateľov s poštovými schránkami v službe Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="31512-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="31512-108">**Krok 2:** Používateľ musí prejsť na kontá **nástrojov**  >  **Accounts**... v Outlooku pre Mac a vyhľadajte a vyberte konto.</span><span class="sxs-lookup"><span data-stu-id="31512-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="31512-109">Potvrďte, že je uvedené meno používateľa vo formáte UPN (napríklad [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="31512-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="31512-110">**Krok 3:** Potvrďte, že používateľ je licencovaným používateľom aplikácie Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="31512-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="31512-111">Používateľ musí používať predplatné na Office 365 pre Mac, verziu produktu 16,24 alebo novšiu verziu.</span><span class="sxs-lookup"><span data-stu-id="31512-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>