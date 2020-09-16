---
title: 'AIP: politiky sa nesprávajú podľa očakávaní'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663204"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="375eb-102">AIP: politiky sa nesprávajú podľa očakávaní</span><span class="sxs-lookup"><span data-stu-id="375eb-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="375eb-103">Azure ochrana informácií: politiky, ktoré sa nesprávajú podľa očakávaní, nájdete v téme Odporúčané pokyny pre rôzne politické problémy:</span><span class="sxs-lookup"><span data-stu-id="375eb-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="375eb-104">Ak máte problémy s vizuálnymi značkami, skontrolujte, či [sa používajú vizuálne označenia](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="375eb-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="375eb-105">Ak máte problémy s automatickým označovaním, prečítajte [si tému Konfigurovanie podmienok pre automatickú a odporúčanú klasifikáciu na ochranu informácií Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a informácie o tom, [ktoré typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)vyhľadávajú.</span><span class="sxs-lookup"><span data-stu-id="375eb-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="375eb-106">Ak máte problémy s natívnou alebo Pfile ochranou, skontrolujte [konfiguráciu konfigurácie súboru API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="375eb-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="375eb-107">Skontrolujte, či používate politiky rozsahu, ktoré nie sú správne nakonfigurované: [Konfigurácia politiky ochrany informácií Azure pre konkrétnych používateľov pomocou politiky rozsahu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="375eb-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="375eb-108">Ak automatické označenie nefunguje pre Outlook pri priložení označeného dokumentu, overte, či DRMEncryptProperty nie je definovaný, ako je to popísané nižšie: [nastavenia databázy Registry IRM pre zabezpečenie](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="375eb-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="375eb-109">Ak sa stále vyskytujú problémy, Zhromaždite denníky klienta Azure Information Protection a priložte exportované denníky do tejto letenky.</span><span class="sxs-lookup"><span data-stu-id="375eb-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="375eb-110">Otvorte dokument balíka Office alebo vytvorte nový e-mail v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="375eb-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="375eb-111">Kliknite na položku **Ochrana**  >  **a citlivosť a pripomienky**.</span><span class="sxs-lookup"><span data-stu-id="375eb-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="375eb-112">Kliknite na položku **Exportovať denníky**.</span><span class="sxs-lookup"><span data-stu-id="375eb-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="375eb-113">Uložte denníky podľa vlastného výberu umiestnenia a priložte ich k tejto žiadosti o službu.</span><span class="sxs-lookup"><span data-stu-id="375eb-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="375eb-114">Ďalšie zdroje:</span><span class="sxs-lookup"><span data-stu-id="375eb-114">Additional resources:</span></span>

- [<span data-ttu-id="375eb-115">Konfigurácia označenia vizuálnych označení na ochranu informácií v službe Azure</span><span class="sxs-lookup"><span data-stu-id="375eb-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="375eb-116">Revízia dokumentácie služby Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="375eb-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="375eb-117">Používanie označení citlivosti v aplikáciách Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="375eb-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

