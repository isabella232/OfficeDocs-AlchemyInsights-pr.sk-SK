---
title: 'AIP: Politiky sa nesprávajú podľa očakávania'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821642"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="9af4c-102">AIP: Politiky sa nesprávajú podľa očakávania</span><span class="sxs-lookup"><span data-stu-id="9af4c-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="9af4c-103">Azure Information Protection: Politiky sa nesprávajú podľa očakávaní, v nasledujúcich odporúčaných pokynoch pre rôzne problémy s politikami:</span><span class="sxs-lookup"><span data-stu-id="9af4c-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="9af4c-104">Ak máte problémy so vizuálnymi označeniami, pozrite si [položku Pri použití vizuálnych označení.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="9af4c-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="9af4c-105">Ak máte problémy s automatickým označením, pozrite si témy Konfigurácia podmienok pre automatickú a odporúčanú klasifikáciu služby [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a Čo hľadia typy [citlivých informácií.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="9af4c-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="9af4c-106">Ak máte problémy s ochranou natívneho súboru alebo súboru Pfile, pozrite si [konfiguráciu rozhrania API súboru.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="9af4c-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="9af4c-107">Skontrolujte, či používate politiky rozsahov, ktoré nie sú správne [nakonfigurované:](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)Konfigurácia politiky Azure Information Protection pre konkrétnych používateľov pomocou politík s rozsahom .</span><span class="sxs-lookup"><span data-stu-id="9af4c-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="9af4c-108">Ak automatické označovanie nefunguje pre Outlook pri priložení označeného dokumentu, overte, či nie je možnosť DRMEncryptProperty definovaná podľa popisu v tomto článku: Nastavenia IRM databázy [Registry pre zabezpečenie.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="9af4c-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="9af4c-109">Ak problémy aj naďalej pretrváva, zhromaždite denníky klientov Azure Information Protection a priložte exportované denníky k tejto lístku.</span><span class="sxs-lookup"><span data-stu-id="9af4c-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="9af4c-110">Otvorte dokument balíka Office alebo vytvorte nový e-mail v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="9af4c-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="9af4c-111">Kliknite **na položku Pomocník a pripomienky k ochrane** alebo  >  **citlivosti.**</span><span class="sxs-lookup"><span data-stu-id="9af4c-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="9af4c-112">Kliknite na **položku Exportovať denníky**.</span><span class="sxs-lookup"><span data-stu-id="9af4c-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="9af4c-113">Uložte denníky podľa vášho výberu a priložte ich k tejto žiadosti o službu.</span><span class="sxs-lookup"><span data-stu-id="9af4c-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="9af4c-114">Ďalšie zdroje:</span><span class="sxs-lookup"><span data-stu-id="9af4c-114">Additional resources:</span></span>

- [<span data-ttu-id="9af4c-115">Konfigurácia označenia pre vizuálne označenia pre Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="9af4c-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="9af4c-116">Kontrola dokumentácie služby Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="9af4c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="9af4c-117">Použitie označení citlivosti v aplikáciách služby Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9af4c-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

