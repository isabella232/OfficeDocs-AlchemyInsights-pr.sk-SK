---
title: 'AIP Scanner: Inštalácia a konfigurácia'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358564"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="75b0a-102">AIP Scanner: Inštalácia a konfigurácia</span><span class="sxs-lookup"><span data-stu-id="75b0a-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="75b0a-103">**Ak chcete nainštalovať skener AIP, postupujte podľa odporúčaných pokynov**:</span><span class="sxs-lookup"><span data-stu-id="75b0a-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="75b0a-104">Ak vykonávate inováciu a nevykonávate čistú inštaláciu, uistite sa, že ste postupovali v pokynoch na [inováciu skenera Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) a pre klienta zjednoteného označovania, pozrite si [Aktualizácia skenera Azure Information Protection Scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="75b0a-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="75b0a-105">Overte, či ste v súlade so všetkými [požiadavkami na nastavenie brány firewall a sieťovej infraštruktúry](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="75b0a-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="75b0a-106">Uistite sa, že vaše [politiky sú nastavené](https://docs.microsoft.com/azure/information-protection/configure-policy) na automatické označovanie alebo majú predvolenú menovku v politike.</span><span class="sxs-lookup"><span data-stu-id="75b0a-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="75b0a-107">Uistite sa, že príslušný typ súboru je nakonfigurovaný na označenie/ochrana, ako je popísané v [typy súborov podporovaných Azure informácie ochrana klienta](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="75b0a-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="75b0a-108">Okrem toho, ak chcete zmeniť predvolené správanie, postupujte podľa týchto pokynov: [Zmena predvolenej úrovne ochrany súborov](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="75b0a-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="75b0a-109">Overte, či používateľské konto nakonfigurované na spustenie služby skener má povolenia na prístup ku všetkým nakonfigurovaným úložiskách.</span><span class="sxs-lookup"><span data-stu-id="75b0a-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="75b0a-110">Ak sa problémy stále vyskytnú, exportujte denníky skenera a pridajte ich do svojho lístka podpory.</span><span class="sxs-lookup"><span data-stu-id="75b0a-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="75b0a-111">**Exportovať denníky Azure informácie ochrany skenera**</span><span class="sxs-lookup"><span data-stu-id="75b0a-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="75b0a-112">Prejdite na%localappdata%\Microsoft\MSIP v kontexte používateľa so službou skener.</span><span class="sxs-lookup"><span data-stu-id="75b0a-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="75b0a-113">ZIP všetok obsah v priečinku MSIP.</span><span class="sxs-lookup"><span data-stu-id="75b0a-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="75b0a-114">Uložte protokoly podľa vášho výberu polohy a priložte ich k požiadavke na službu.</span><span class="sxs-lookup"><span data-stu-id="75b0a-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="75b0a-115">Môžete tiež použiť [export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="75b0a-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="75b0a-116">**Ďalšie informácie nájdete v téme**:</span><span class="sxs-lookup"><span data-stu-id="75b0a-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="75b0a-117">Nasadenie Azure Information Protection Scanner automaticky klasifikovať a chrániť súbory</span><span class="sxs-lookup"><span data-stu-id="75b0a-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="75b0a-118">Zadajte a použite token parameter pre overovanie set-AIP</span><span class="sxs-lookup"><span data-stu-id="75b0a-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="75b0a-119">Spustenie cyklu zisťovania a zobrazenie zostáv pre skener</span><span class="sxs-lookup"><span data-stu-id="75b0a-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="75b0a-120">Preskúmanie Azure informácie o ochrane dokumentácie</span><span class="sxs-lookup"><span data-stu-id="75b0a-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="75b0a-121">Požiadavky na Azure informácie o ochrane</span><span class="sxs-lookup"><span data-stu-id="75b0a-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="75b0a-122">Stiahnuť Azure informácie o ochrane klienta</span><span class="sxs-lookup"><span data-stu-id="75b0a-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
