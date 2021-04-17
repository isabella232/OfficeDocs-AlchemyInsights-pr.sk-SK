---
title: Migrácia z AIP na označenie MIP alebo zjednotené označenie v Centre dodržiavania súladu
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825386"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="ff9af-102">Migrácia z AIP na označenie MIP alebo zjednotené označenie v Centre dodržiavania súladu</span><span class="sxs-lookup"><span data-stu-id="ff9af-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="ff9af-103">Ak chcete migrovať z označení AIP do zjednoteného označenia v centre zabezpečenia a dodržiavania súladu, vykonajte nasledovné:</span><span class="sxs-lookup"><span data-stu-id="ff9af-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="ff9af-104">**Aktivácia zabezpečenia z portálu Azure**</span><span class="sxs-lookup"><span data-stu-id="ff9af-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="ff9af-105">Ak ste tak ešte neurobili, otvorte nové okno prehliadača a [prihláste sa na portál Azure.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="ff9af-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="ff9af-106">Prejdite na **blade Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="ff9af-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="ff9af-107">Napríklad v ponuke Centrum kliknite na položku **Všetky služby** a do poľa Filter **začnite** zadávať informácie.</span><span class="sxs-lookup"><span data-stu-id="ff9af-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="ff9af-108">Vyberte **položku Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="ff9af-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="ff9af-109">Ak ste doteraz nemali prístup k aplikácii Azure Information [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) Protection, pozrite si jednočasové ďalšie kroky na pridanie tohto blade na portál.</span><span class="sxs-lookup"><span data-stu-id="ff9af-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="ff9af-110">Ak chcete otvoriť aplikáciu Azure Information Protection blade, musíte mať buď plán [Azure Information Protection Premium,](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) alebo plán služieb Office 365, ktorý obsahuje správu prístupových práv.</span><span class="sxs-lookup"><span data-stu-id="ff9af-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="ff9af-111">Ak máte niektoré z týchto predplatných, ale zobrazuje sa hlásenie, že platné predplatné nie je možné nájsť, obráťte sa na technickú podporu spoločnosti [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) alebo použite štandardné kanály podpory.</span><span class="sxs-lookup"><span data-stu-id="ff9af-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="ff9af-112">Vyhľadajte možnosti **ponuky Spravovať** a vyberte položku **Aktivácia zabezpečenia**.</span><span class="sxs-lookup"><span data-stu-id="ff9af-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="ff9af-113">Kliknite **na položku** Aktivovať a potom potvrďte akciu.</span><span class="sxs-lookup"><span data-stu-id="ff9af-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="ff9af-114">Po dokončení aktivácie sa na informačnom paneli zobrazí hlásenie **Aktivácia sa úspešne dokončila.**</span><span class="sxs-lookup"><span data-stu-id="ff9af-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="ff9af-115">**Migrácia označení Azure Information Protection do Centra zabezpečenia a dodržiavania & Office 365**</span><span class="sxs-lookup"><span data-stu-id="ff9af-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="ff9af-116">Prihláste sa ako používateľ s povolením globálneho správcu.</span><span class="sxs-lookup"><span data-stu-id="ff9af-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="ff9af-117">Prejdite na **blade Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="ff9af-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="ff9af-118">V ponuke **Spravovať** vyberte položku **Zjednotené označovanie**.</span><span class="sxs-lookup"><span data-stu-id="ff9af-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="ff9af-119">Na obrazovke **Azure Information Protection – Unified labeling** blade kliknite na položku **Aktivovať a** postupujte podľa online pokynov.</span><span class="sxs-lookup"><span data-stu-id="ff9af-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="ff9af-120">**Poznámka:** Pred aktiváciou migrácie Centra zabezpečenia a dodržiavania súladu overte, či & príslušné povolenia.</span><span class="sxs-lookup"><span data-stu-id="ff9af-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="ff9af-121">Ďalšie informácie nájdete v týchto článkoch:</span><span class="sxs-lookup"><span data-stu-id="ff9af-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="ff9af-122">Potrebujete byť globálnym správcom na konfiguráciu služby Azure Information Protection alebo môžem delegovať na iných správcov?</span><span class="sxs-lookup"><span data-stu-id="ff9af-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="ff9af-123">Dôležité informácie o rolách správcu po migrácii do centra zabezpečenia & súladu.</span><span class="sxs-lookup"><span data-stu-id="ff9af-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="ff9af-124">Ďalšie informácie o AIP do zjednotenej migrácie označení do Centra zabezpečenia a dodržiavania súladu nájdete v téme [Migrácia označení.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="ff9af-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
