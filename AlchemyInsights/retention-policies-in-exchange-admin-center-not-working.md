---
title: Politiky uchovávania údajov v Centre spravovania pre Exchange nefungujú
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952243"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="3edea-102">Politiky uchovávania údajov v Centre spravovania pre Exchange</span><span class="sxs-lookup"><span data-stu-id="3edea-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="3edea-103">Ak chcete, aby sme spúšťali automatizované kontroly nižšie uvedených nastavení, vyberte tlačidlo Späť < – v hornej časti tejto stránky a potom zadajte e-mailovú adresu používateľa, ktorý má problémy s politikami uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="3edea-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="3edea-104">Ak máte problémy s politikami uchovávania údajov, ktoré sa v Centre spravovania pre Exchange vzťahujú na poštové schránky a položky, ktoré sa nepresúdnia do archívnej poštovej schránky, skontrolujte toto:</span><span class="sxs-lookup"><span data-stu-id="3edea-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="3edea-105">**Koreňové príčiny:**</span><span class="sxs-lookup"><span data-stu-id="3edea-105">**Root Causes:**</span></span>

- <span data-ttu-id="3edea-106">**Asistent spravovaných** priečinkov nespracová poštovú schránku používateľa.</span><span class="sxs-lookup"><span data-stu-id="3edea-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="3edea-107">Asistent spravovaných priečinkov sa pokúsi spracovať každú poštovú schránku vo vašej cloudovej organizácii raz za sedem dní.</span><span class="sxs-lookup"><span data-stu-id="3edea-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="3edea-108">**Riešenie:** Spustite asistenta spravovaných priečinkov.</span><span class="sxs-lookup"><span data-stu-id="3edea-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="3edea-109">**Funkcia RetentionHold** bola **v poštovej** schránke povolená.</span><span class="sxs-lookup"><span data-stu-id="3edea-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="3edea-110">Ak bola poštová schránka umiestnená na umiestnení lokality RetentionHold, politika uchovávania údajov pre poštovú schránku sa počas tohto času nespracuje.</span><span class="sxs-lookup"><span data-stu-id="3edea-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="3edea-111">**Riešenie:** Skontrolujte stav nastavenia uchovávania údajov a aktualizujte ho podľa potreby.</span><span class="sxs-lookup"><span data-stu-id="3edea-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="3edea-112">Podrobnosti nájdete v téme Uchovávanie [údajov v poštovej schránke.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="3edea-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="3edea-113">**Poznámka:** Ak je poštová schránka menšia ako 10 MB, asistent spravovaných priečinkov nebude poštovú schránku automaticky spracovať.</span><span class="sxs-lookup"><span data-stu-id="3edea-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="3edea-114">Ďalšie informácie o politikách uchovávania údajov v Centre spravovania pre Exchange nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="3edea-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="3edea-115">Značky uchovávania údajov a politiky uchovávania údajov</span><span class="sxs-lookup"><span data-stu-id="3edea-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="3edea-116">[Použitie politiky uchovávania údajov pre poštové schránky alebo](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Pridanie alebo odstránenie značiek uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="3edea-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="3edea-117">Ako identifikovať typ zadržanej poštovej schránky</span><span class="sxs-lookup"><span data-stu-id="3edea-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
