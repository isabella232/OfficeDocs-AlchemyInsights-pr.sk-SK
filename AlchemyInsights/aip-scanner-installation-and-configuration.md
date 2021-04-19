---
title: 'Skener AIP: inštalácia a konfigurácia'
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
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821678"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="934df-102">Skener AIP: inštalácia a konfigurácia</span><span class="sxs-lookup"><span data-stu-id="934df-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="934df-103">**Ak chcete nainštalovať skener AIP, postupujte podľa odporúčaných pokynov:**</span><span class="sxs-lookup"><span data-stu-id="934df-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="934df-104">Ak vykonávate inováciu a nevykonáte čistú inštaláciu, skontrolujte, či ste postupovali podľa pokynov na inováciu skenera [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) a pre jednotného klienta označenia, pozrite si inovovanie skenera Azure Information [Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)</span><span class="sxs-lookup"><span data-stu-id="934df-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="934df-105">Overte, či spĺňate všetky [požiadavky na nastavenia brány firewall a sieťovej infraštruktúry.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="934df-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="934df-106">Skontrolujte, či [sú politiky nastavené na](https://docs.microsoft.com/azure/information-protection/configure-policy) automatické označovanie alebo majú v politike predvolené označenie.</span><span class="sxs-lookup"><span data-stu-id="934df-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="934df-107">Presvedčte sa, že príslušný typ súboru je nakonfigurovaný na označenie alebo ochranu podľa popisu v časti Typy súborov podporované klientom [Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="934df-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="934df-108">Okrem toho, ak chcete zmeniť predvolené správanie, postupujte podľa týchto pokynov: [Zmena predvolenej úrovne ochrany súborov](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="934df-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="934df-109">Overte, či používateľské konto nakonfigurované na spustenie služby skenera má povolenia na prístup ku všetkým nakonfigurovaným odklada priestorom.</span><span class="sxs-lookup"><span data-stu-id="934df-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="934df-110">Ak problémy pretrváva, exportujte denníky skenerov a pridajte ich do lístka technickej podpory.</span><span class="sxs-lookup"><span data-stu-id="934df-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="934df-111">**Exportovanie denníkov skenera informácií Azure**</span><span class="sxs-lookup"><span data-stu-id="934df-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="934df-112">V kontexte používateľa služby skenera prejdite na položku %localappdata%\Microsoft\MSIP.</span><span class="sxs-lookup"><span data-stu-id="934df-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="934df-113">Komprimujte celý obsah pod priečinok MSIP.</span><span class="sxs-lookup"><span data-stu-id="934df-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="934df-114">Uložte denníky podľa vášho výberu a priložte ich k žiadosti o službu.</span><span class="sxs-lookup"><span data-stu-id="934df-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="934df-115">Môžete tiež použiť [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="934df-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="934df-116">**Ďalšie informácie nájdete v téme:**</span><span class="sxs-lookup"><span data-stu-id="934df-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="934df-117">Nasadenie skenera Azure Information Protection na automatické klasifikáciu a ochranu súborov</span><span class="sxs-lookup"><span data-stu-id="934df-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="934df-118">Zadanie a použitie parametra Token pre Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="934df-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="934df-119">Spustenie cyklu zisťovania a zobrazenie zostáv pre skener</span><span class="sxs-lookup"><span data-stu-id="934df-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="934df-120">Kontrola dokumentácie služby Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="934df-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="934df-121">Požiadavky na službu Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="934df-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="934df-122">Stiahnutie klienta Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="934df-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
