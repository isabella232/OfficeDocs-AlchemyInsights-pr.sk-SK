---
title: Politiky hesiel
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747052"
---
# <a name="password-policies"></a><span data-ttu-id="03701-102">Politiky hesiel</span><span class="sxs-lookup"><span data-stu-id="03701-102">Password policies</span></span>

<span data-ttu-id="03701-103">**Mám problémy s politikou hesla používateľa**</span><span class="sxs-lookup"><span data-stu-id="03701-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="03701-104">Politika hesiel pre používateľa závisí od toho, či je používateľ iba v cloude alebo lokálne.</span><span class="sxs-lookup"><span data-stu-id="03701-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="03701-105">Iba cloud používatelia si musia vybrať heslo, ktoré spĺňa požiadavky uvedené v tomto článku: [politiky hesla, ktoré sa používajú len v cloudových používateľských kontách](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts) .</span><span class="sxs-lookup"><span data-stu-id="03701-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="03701-106">Lokálni používatelia musia vybrať heslo, ktoré spĺňa lokálne požiadavky.</span><span class="sxs-lookup"><span data-stu-id="03701-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="03701-107">Ak lokálny používateľ nedokáže nastaviť svoje heslo, skontrolujte svoje lokálne požiadavky.</span><span class="sxs-lookup"><span data-stu-id="03701-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="03701-108">**Neviem, ako nastaviť alebo skontrolovať politiky uplynutia platnosti hesla**</span><span class="sxs-lookup"><span data-stu-id="03701-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="03701-109">Pomocou prostredia PowerShell môžete nastaviť a skontrolovať politiku uplynutia platnosti pre používateľov cloudu v nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="03701-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="03701-110">Postupujte podľa pokynov v tomto článku: [Nastavenie alebo kontrola politiky hesiel pomocou prostredia PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="03701-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="03701-111">Politika uplynutia platnosti hesla pre lokálnych používateľov je nastavená v lokálnej REKLAMe.</span><span class="sxs-lookup"><span data-stu-id="03701-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="03701-112">**Ďalšie užitočné prepojenia:**</span><span class="sxs-lookup"><span data-stu-id="03701-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="03701-113">Začíname s vytvorením nového hesla</span><span class="sxs-lookup"><span data-stu-id="03701-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="03701-114">Riešenie problémov s vynulovaním hesla iniciovaného správcom</span><span class="sxs-lookup"><span data-stu-id="03701-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
