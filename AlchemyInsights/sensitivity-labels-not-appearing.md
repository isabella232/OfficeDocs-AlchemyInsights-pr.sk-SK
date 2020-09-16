---
title: Označenia citlivosti sa nezobrazujú
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801199"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="b74fc-102">Označenia citlivosti sa nezobrazujú</span><span class="sxs-lookup"><span data-stu-id="b74fc-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="b74fc-103">Označenia citlivosti umožňujú klasifikáciu a ochranu citlivého obsahu.</span><span class="sxs-lookup"><span data-stu-id="b74fc-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="b74fc-104">Dajú sa vytvoriť v centre zabezpečenia dodržiavania súladu pre Microsoft 365, v centre zabezpečenia spoločnosti Microsoft 365 alebo v centre zabezpečenia spoločnosti Microsoft & 365 v časti klasifikácie > označenia citlivosti.</span><span class="sxs-lookup"><span data-stu-id="b74fc-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="b74fc-105">Ďalšie informácie o tejto funkcii nájdete v téme [Prehľad označení citlivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="b74fc-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="b74fc-106">Ak ste nakonfigurovali označenia citlivosti, ale nezobrazujú sa v aplikáciách Microsoft 365, skontrolujte nasledovné:</span><span class="sxs-lookup"><span data-stu-id="b74fc-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="b74fc-107">Potvrďte, že označenie citlivosti bolo [zverejnené](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) používateľom a skupinám, ktoré chcete.</span><span class="sxs-lookup"><span data-stu-id="b74fc-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="b74fc-108">Potvrďte, že používateľ používa aplikáciu, ktorá podporuje označenia citlivosti – Pozrite si tému [označenia citlivosti v dokumente](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="b74fc-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="b74fc-109">Ak chcete [migrovať označenia Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), uvedomte si [tu](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)uvedené úvahy.</span><span class="sxs-lookup"><span data-stu-id="b74fc-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="b74fc-110">Podpora ochrany pred únikom údajov (DLP): momentálne je v politikách DLP možné použiť len označenia uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="b74fc-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="b74fc-111">Podpora označení citlivosti v politike DLP zatiaľ nie je k dispozícii, ale na nej pracujeme.</span><span class="sxs-lookup"><span data-stu-id="b74fc-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="b74fc-112">Ak je šifrovanie zapnuté na označení citlivosti, môžete si vybrať buď:</span><span class="sxs-lookup"><span data-stu-id="b74fc-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="b74fc-113">Priradenie povolení</span><span class="sxs-lookup"><span data-stu-id="b74fc-113">Assign permissions now</span></span>
    - <span data-ttu-id="b74fc-114">Umožnenie používateľom priraďovať povolenia</span><span class="sxs-lookup"><span data-stu-id="b74fc-114">Let users assign permissions</span></span>


<span data-ttu-id="b74fc-115">Ďalšie informácie o možných problémoch nájdete v téme [známe problémy s menovkami citlivosti](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="b74fc-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>