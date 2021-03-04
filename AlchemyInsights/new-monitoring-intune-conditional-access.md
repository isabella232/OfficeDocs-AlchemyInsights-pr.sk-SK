---
title: Monitorovanie podmieneného prístupu služby Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428306"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="96011-102">Monitorovanie podmieneného prístupu služby Intune</span><span class="sxs-lookup"><span data-stu-id="96011-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="96011-103">Používatelia s podmieneným prístupom budú dostávať e-maily s upozornením, ak nespĺňajú požiadavky na prístup vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="96011-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="96011-104">Ak chcete vyriešiť, odporúčame niektoré z týchto riešení:</span><span class="sxs-lookup"><span data-stu-id="96011-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="96011-105">Ak sa predpokladá, že zariadenie je zaregistrované, odporúča sa používateľovi prejsť na aplikáciu firemný portál a overiť, či sa zobrazuje na firemnom portáli.</span><span class="sxs-lookup"><span data-stu-id="96011-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="96011-106">Ak to tak nie je, používateľ musí zaregistrovať zariadenie.</span><span class="sxs-lookup"><span data-stu-id="96011-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="96011-107">Na portáli Azure prejdite na   >  **súlad zariadenia** so službou Intune.</span><span class="sxs-lookup"><span data-stu-id="96011-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="96011-108">Ak chcete zobraziť zostavu súladu zariadenia a overiť, či je zariadenie používateľa označené ako vyhovujúce, v časti **Monitor** kliknite na položku **zhoda zariadení**.</span><span class="sxs-lookup"><span data-stu-id="96011-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="96011-109">Na portáli Azure prejdite na   >  **súlad zariadenia** so službou Intune.</span><span class="sxs-lookup"><span data-stu-id="96011-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="96011-110">V časti **Spravovať** kliknite na položku **politiky**.</span><span class="sxs-lookup"><span data-stu-id="96011-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="96011-111">V zozname politík dodržiavania súladu Skontrolujte, či je profil priradený k zariadeniu používateľa.</span><span class="sxs-lookup"><span data-stu-id="96011-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="96011-112">Ak nie je priradený žiadny profil, služby Intune nebudú môcť potvrdiť stav súladu zariadenia.</span><span class="sxs-lookup"><span data-stu-id="96011-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="96011-113">Upravte priradenie podmieneného prístupu používateľa.</span><span class="sxs-lookup"><span data-stu-id="96011-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="96011-114">Na portáli Azure prejdite do   >  časti politiky **podmieneného prístupu** služby Intune  >  , vyberte politiku v zozname a kliknite na položku **Používatelia a skupiny**.</span><span class="sxs-lookup"><span data-stu-id="96011-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="96011-115">Ak chcete určitú politiku zacieliť na inú osobu, pridajte ich do **zoznamu zahrnúť**.</span><span class="sxs-lookup"><span data-stu-id="96011-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="96011-116">Ak chcete zabezpečiť, aby bola osoba z politiky vynechaná, pridajte ju do **zoznamu výnimiek**.</span><span class="sxs-lookup"><span data-stu-id="96011-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="96011-117">**Užitočné prepojenia:**</span><span class="sxs-lookup"><span data-stu-id="96011-117">**Helpful links:**</span></span>

- [<span data-ttu-id="96011-118">Prehľad súladu zariadenia</span><span class="sxs-lookup"><span data-stu-id="96011-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="96011-119">Riešenie problémov s certifikačnou autoritou</span><span class="sxs-lookup"><span data-stu-id="96011-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="96011-120">Politika riešenia problémov</span><span class="sxs-lookup"><span data-stu-id="96011-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="96011-121">Sledovanie dodržiavania súladu zariadenia Intune</span><span class="sxs-lookup"><span data-stu-id="96011-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="96011-122">Tieto kroky sú užitočné len pri riešení problémov s podmieneným prístupom funkcie Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="96011-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="96011-123">Je tiež možné do karantény zablokovať zariadenie, ktoré blokuje prístup k e-mailu pomocou politiky Exchange.</span><span class="sxs-lookup"><span data-stu-id="96011-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="96011-124">Ďalšie informácie o správe zariadenia Exchange nájdete [**tu**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="96011-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
