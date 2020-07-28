---
title: Viaceré objekty majú rovnakú e-mailovú adresu ako identita
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439711"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="f8c6e-102">Viaceré objekty majú rovnakú e-mailovú adresu ako identita</span><span class="sxs-lookup"><span data-stu-id="f8c6e-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="f8c6e-103">**Viaceré objekty**</span><span class="sxs-lookup"><span data-stu-id="f8c6e-103">**Multiple objects**</span></span>

<span data-ttu-id="f8c6e-104">Jedným z bežných dôvodov tejto chyby nie je možné správne smerovať požiadavku služby Outlook Web Access v prítomnosti viacerých objektov s rovnakou e-mailovú adresu ako identita.</span><span class="sxs-lookup"><span data-stu-id="f8c6e-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="f8c6e-105">Ak chcete nájsť tieto objekty, spustite nasledujúce príkazy:</span><span class="sxs-lookup"><span data-stu-id="f8c6e-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="f8c6e-106">· Získať príjemcu<email address></span><span class="sxs-lookup"><span data-stu-id="f8c6e-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="f8c6e-107">· Získať používateľa<email address></span><span class="sxs-lookup"><span data-stu-id="f8c6e-107">· Get-User <email address></span></span>

<span data-ttu-id="f8c6e-108">· Získajte užívateľa <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="f8c6e-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="f8c6e-109">· Získať kontakt<email address></span><span class="sxs-lookup"><span data-stu-id="f8c6e-109">· Get-Contact <email address></span></span>

<span data-ttu-id="f8c6e-110">· Získať poštovej <email address> schránky - PublicFolder</span><span class="sxs-lookup"><span data-stu-id="f8c6e-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="f8c6e-111">· Získať poštovej <email address> schránky - IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="f8c6e-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="f8c6e-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="f8c6e-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="f8c6e-113">Ak chcete vyriešiť tento problém, odstráňte viaceré objekty s rovnakou e-mailovú identitu a uistite sa, že existuje jeden objekt s konkrétnou e-mailovú identitu a že jeho typ príjemcu je UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="f8c6e-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="f8c6e-114">**Rovnaká adresa sa používa pre obchodné a spotrebiteľské poštové schránky**</span><span class="sxs-lookup"><span data-stu-id="f8c6e-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="f8c6e-115">Ďalšou príčinou je, keď sa rovnaká adresa používa pre obchodné a spotrebiteľské poštové schránky.</span><span class="sxs-lookup"><span data-stu-id="f8c6e-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="f8c6e-116">V tomto prípade musí používateľ zmeniť svoj primárny spotrebiteľský alias, kým Cafe podporuje tento scenár.</span><span class="sxs-lookup"><span data-stu-id="f8c6e-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="f8c6e-117">Ide o trvalú chybu, ktorá nezmizne bez zásahu.</span><span class="sxs-lookup"><span data-stu-id="f8c6e-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="f8c6e-118">Podrobnosti nájdete v téme [Zmena e-mailovej adresy alebo telefónneho čísla konta Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="f8c6e-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>