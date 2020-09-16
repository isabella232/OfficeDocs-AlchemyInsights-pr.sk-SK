---
title: Migrácia z AIP na MDC/zjednotené označenie v centre dodržiavania súladu
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674341"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="0755f-102">Migrácia z AIP na MDC/zjednotené označenie v centre dodržiavania súladu</span><span class="sxs-lookup"><span data-stu-id="0755f-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="0755f-103">Ak chcete migrovať z menoviek AIP na zjednotené označenie v centre zabezpečenia a dodržiavania súladu, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="0755f-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="0755f-104">**Aktivácia ochrany na portáli Azure**</span><span class="sxs-lookup"><span data-stu-id="0755f-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="0755f-105">Ak ste to ešte neurobili, Otvorte nové okno prehliadača a [Prihláste sa na portáli Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="0755f-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="0755f-106">Prejdite na čepeľ na **ochranu informácií v Azure** .</span><span class="sxs-lookup"><span data-stu-id="0755f-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="0755f-107">V ponuke rozbočovač kliknite napríklad na položku **všetky služby** a začnite písať **informácie** do poľa Filter.</span><span class="sxs-lookup"><span data-stu-id="0755f-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="0755f-108">Vyberte položku **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="0755f-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="0755f-109">Ak ste sa ešte nedostali do programu Azure Information Protection Blade, pozrite si jednorazové [Ďalšie kroky](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) na pridanie tohto kotúča na portál.</span><span class="sxs-lookup"><span data-stu-id="0755f-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="0755f-110">Ak chcete otvoriť čepeľ na ochranu informácií o Azure, musíte mať [plán služieb Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) alebo plán služieb Office 365, ktorý obsahuje správu prístupových práv.</span><span class="sxs-lookup"><span data-stu-id="0755f-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="0755f-111">Ak máte niektorý z týchto predplatných, ale zobrazí sa hlásenie o tom, že platné predplatné sa nenašlo, obráťte sa na oddelenie technickej podpory [spoločnosti Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) alebo použite štandardné podporné kanály.</span><span class="sxs-lookup"><span data-stu-id="0755f-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="0755f-112">Vyhľadajte možnosti ponuky **Spravovať** a vyberte položku **Aktivácia ochrany**.</span><span class="sxs-lookup"><span data-stu-id="0755f-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="0755f-113">Kliknite na položku **aktivovať**a potvrďte akciu.</span><span class="sxs-lookup"><span data-stu-id="0755f-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="0755f-114">Po dokončení aktivácie sa na informačnom paneli zobrazí hlásenie **Aktivácia sa úspešne dokončila**.</span><span class="sxs-lookup"><span data-stu-id="0755f-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="0755f-115">**Migrácia menoviek Azure Information Protection na centrum zabezpečenia & zabezpečenia dodržiavania súladu v Office 365**</span><span class="sxs-lookup"><span data-stu-id="0755f-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="0755f-116">Skontrolujte, či ste prihlásení ako používateľ s povolením globálneho správcu.</span><span class="sxs-lookup"><span data-stu-id="0755f-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="0755f-117">Prejdite na čepeľ na **ochranu informácií v Azure** .</span><span class="sxs-lookup"><span data-stu-id="0755f-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="0755f-118">V ponuke **Spravovať** vyberte možnosť **Unified labeling (zjednotené označenie**).</span><span class="sxs-lookup"><span data-stu-id="0755f-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="0755f-119">Na karte **Azure Information Protection – Unified labeling** Blade kliknite na položku **aktivovať** a postupujte podľa pokynov online.</span><span class="sxs-lookup"><span data-stu-id="0755f-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="0755f-120">**Poznámka**: Skontrolujte, či máte príslušné povolenia pred aktiváciou migrácie centra zabezpečenia & súladu.</span><span class="sxs-lookup"><span data-stu-id="0755f-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="0755f-121">Ďalšie informácie nájdete v týchto článkoch:</span><span class="sxs-lookup"><span data-stu-id="0755f-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="0755f-122">Musíte byť globálnym správcom na konfiguráciu služby Azure Information Protection alebo môžem delegovať na iných správcov?</span><span class="sxs-lookup"><span data-stu-id="0755f-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="0755f-123">Dôležité informácie o rolách správcu po migrácii do centra zabezpečenia & dodržiavania súladu.</span><span class="sxs-lookup"><span data-stu-id="0755f-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="0755f-124">Ďalšie informácie o AIP na zjednotené označenie migrácie do centra zabezpečenia a dodržiavania súladu nájdete v téme [migrácia menoviek](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="0755f-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
