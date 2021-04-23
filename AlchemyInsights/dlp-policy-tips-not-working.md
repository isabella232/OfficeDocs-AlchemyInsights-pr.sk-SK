---
title: Politika DLP nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 68387bf6f5f91657f1d853b9d67bdea6fac21bde
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952207"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="62d9b-102">Problémy s policy Tipom pre DLP</span><span class="sxs-lookup"><span data-stu-id="62d9b-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="62d9b-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="62d9b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="62d9b-104">Ak chcete nakonfigurovať tipy k politike DLP v centre zabezpečenia & dodržiavania súladu v režime úplného vynútenia, vykonajte nasledovné kroky:</span><span class="sxs-lookup"><span data-stu-id="62d9b-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="62d9b-105">Uistite sa, že v **pravidle** DLP sú povolené tipy k politike.</span><span class="sxs-lookup"><span data-stu-id="62d9b-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="62d9b-106">Postup nájdete v téme [Odosielanie e-mailových oznámení a zobrazenie tipov na politiky DLP.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="62d9b-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="62d9b-107">Skontrolujte, či obsah zodpovedá tomu, čo je potrebné na spustenie pravidla uvedeného v [definíciách entít typu Citlivé informácie.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="62d9b-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

<span data-ttu-id="62d9b-108">Zobrazovanie tipov na politiky v aplikácii OWA aj v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="62d9b-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="62d9b-109">Ak však používate Outlook 2013 alebo novšiu verziu, tipy k politike sa zobrazia len za určitých podmienok.</span><span class="sxs-lookup"><span data-stu-id="62d9b-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="62d9b-110">Konkrétny zoznam podmienok nájdete v téme Podporované [podmienky pre Outlook 2013 alebo novšiu verziu,](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)v ktorých nájdete tipy k politike.</span><span class="sxs-lookup"><span data-stu-id="62d9b-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="62d9b-111">Informácie o tipoch na politiky DLP nájdete v téme [Tipy k politike DLP – referenčná](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) matica a matica podpory [pre tipy k politike DLP.](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)</span><span class="sxs-lookup"><span data-stu-id="62d9b-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>