---
title: Zobrazuje sa mi blokovanie podmieneným prístupom k zariadeniam pripojenému k doméne
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038102"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="0d7cf-102">Zobrazuje sa mi blokovanie podmieneným prístupom k zariadeniam pripojenému k doméne</span><span class="sxs-lookup"><span data-stu-id="0d7cf-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="0d7cf-103">**Veľmi odporúčaná nástroje**</span><span class="sxs-lookup"><span data-stu-id="0d7cf-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="0d7cf-104">[Nástroj na riešenie problémov s registráciou zariadenia](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – nástroj, ktorý pomáha pri riešení bežných problémov s registráciou zariadenia.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="0d7cf-105">[Otestujte skript pripojenia k registrácii zariadenia](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – skript, ktorý pomáha zabezpečiť, že zariadenie môže získať prístup ku koncovým bodom registrácie zariadenia pod systémovým kontom.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="0d7cf-106">[Skript čistenia zariadenia Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) – skript, ktorý umožňuje vyhľadávať a spravovať zastarané zariadenia vo vašom prostredí.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="0d7cf-107">Tu je niekoľko bežných dôvodov, prečo podmienený prístup môže zlyhať v zariadení, ktoré sa pripojilo k doméne (hybridná Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0d7cf-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="0d7cf-108">**V zariadení nie je k dispozícii žiadne služby Azure AD PRT** – je potrebné zabezpečiť, aby zariadenie vytvorilo token primárneho obnovenia Azure AD (PRT).</span><span class="sxs-lookup"><span data-stu-id="0d7cf-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="0d7cf-109">Ďalšie informácie o PRT nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="0d7cf-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="0d7cf-110">Ak chcete overiť, či máte službu Azure AD PRT, môžete spustiť `dsregcmd/status` príkaz v zariadení a overiť, či sa "AzureAdPrt" rovná "Yes" (Áno).</span><span class="sxs-lookup"><span data-stu-id="0d7cf-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="0d7cf-111">Ak je argument "AzureAdPrt" "nie", skontrolujte nasledovné:</span><span class="sxs-lookup"><span data-stu-id="0d7cf-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="0d7cf-112">**Či máte externé prostredie so službou AD FS a nie je dosiahnuteľné od domácich sietí používateľov**: v tomto prípade skontrolujte, či sú koncové body "usernamemixed" prístupné z extranetu.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="0d7cf-113">Ak sa vaša AD FS nachádza za VPN, zabezpečte, aby sa používatelia pripojili k sieti VPN a opätovne sa prihlásili do zariadenia.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="0d7cf-114">Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="0d7cf-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="0d7cf-115">**Či je modul TPM zariadenia chybný, a preto nedokáže overiť zariadenie**: začiarknite políčko TPM. msc a zistite, či je stav modulu TPM pripravený.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="0d7cf-116">Ak to tak nie je, spustite `dsregcmd/leave` a nechajte zariadenie opätovne pripájať sa k službe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="0d7cf-117">Potom skúste to znova.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-117">Then, try again.</span></span> <span data-ttu-id="0d7cf-118">Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="0d7cf-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="0d7cf-119">Používate **poskytovateľa identity tretej strany, ktorý nepodporuje WS-Trust protokol**.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="0d7cf-120">Ako je popísané v našich dokumentoch, hybridné Azure AD-pripojené zariadenia nemôžu v tomto prípade fungovať.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="0d7cf-121">Ak máte pomoc, obráťte sa na svojho poskytovateľa identity.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="0d7cf-122">**Používatelia používajú prehliadač Chrome bez kont Windowsu 10** alebo **Office Extension Chrome automaticky nepoužíva PRT v zariadeniach s funkciou AAD alebo hybridné AAD**: to vedie k zlyhaniu všetkých politík podmieneného prístupu založených na zariadení, pričom sa zobrazí chybové hlásenie neregistrované zariadenie.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="0d7cf-123">Ak chcete používať prehliadač Chrome správne, musíte nainštalovať konto Windows 10 alebo rozšírenie balíka Office do prehliadača Chrome používateľov cez SCCM alebo Intune.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="0d7cf-124">Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="0d7cf-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="0d7cf-125">Ak nie je možné rozšíriť rozšírenie na diaľku, upozorniť používateľov na manuálnu inštaláciu niektorej z vyššie uvedených rozšírení na prístup k aplikáciám za podmieneným prístupom založeným na zariadení.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="0d7cf-126">Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="0d7cf-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="0d7cf-127">**Zariadenie bolo správne pripojené k hybridnej službe Azure AD, ale bolo neúmyselne odstránené alebo vypnuté, a to buď z dôvodu zmeny synchronizácie v službe Azure AD Connect alebo na portáli Azure**: Ak sa to stane, objekt zariadenia sa už nerozpoznal ako úplne pripojené zariadenie, hoci stav "AzureAdJoined" a "PRT" sa v zariadení zobrazuje ako platný.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="0d7cf-128">Ak chcete tento problém vyriešiť, spustite `dsregcmd/leave` príslušné zariadenia a nechajte ich opätovne spojiť so službou Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="0d7cf-129">Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="0d7cf-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="0d7cf-130">Ak sú vaše zariadenia vo Windowse 10, 1809 Update, so serverom VPN/cloud proxy a pozrite si tému problémy so stavom "AzureAdPrt" alebo akoukoľvek aplikáciou s problémom SSO (Outlook sa nepripája k poštovej schránke, aj keď ste mali PRT), uistite sa, že máte tento patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) alebo Kumulatívna aktualizácia [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , aby sa zabránilo zlyhaniu PRT na týchto strojoch.</span><span class="sxs-lookup"><span data-stu-id="0d7cf-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















