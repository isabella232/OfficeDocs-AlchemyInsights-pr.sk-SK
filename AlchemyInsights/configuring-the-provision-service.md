---
title: Konfigurovanie služby zabezpečenia
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484043"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="c6f96-102">Konfigurovanie služby zabezpečenia</span><span class="sxs-lookup"><span data-stu-id="c6f96-102">Configuring the Provision service</span></span>

<span data-ttu-id="c6f96-103">Ak chcete, aby automatizované poskytovanie používateľov fungovalo, Azure AD vyžaduje platné poverenia, ktoré mu umožnia pripojiť sa k službe API pre webové služby v rámci pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="c6f96-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="c6f96-104">Okrem toho sa v aplikácii na poskytovanie služby AD User (skúšobné pripojenie) na stránke pracovný postup overí aj to, či sa používateľ môže pripojiť k agentovi poskytovania služby Azure AD Connect, ktorý je priradený k REKLAMnej doméne.</span><span class="sxs-lookup"><span data-stu-id="c6f96-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="c6f96-105">Ak Azure Portal vráti chybu pri ukladaní poverení, postupujte podľa nižšie uvedených odporúčaných krokov:</span><span class="sxs-lookup"><span data-stu-id="c6f96-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="c6f96-106">Potvrďte, že ste nakonfigurovali používateľské konto na integráciu do pracovného dňa, ako je to uvedené v časti výučba v časti [Konfigurácia používateľa systému integrácie v deň](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="c6f96-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="c6f96-107">Overte, či je služba Azure AD Connect poskytovanie agenta na lokálnom serveri Windowsu spustená pomocou konzoly na správu služieb.</span><span class="sxs-lookup"><span data-stu-id="c6f96-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="c6f96-108">Môžete tiež skontrolovať stav agenta na portáli Azure kliknutím na tlačidlo Zobraziť lokálne agentov.</span><span class="sxs-lookup"><span data-stu-id="c6f96-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="c6f96-109">Uistite sa, že zadávate hodnotu pre pole meno používateľa v textovom poli s použitím formátu username@workday – meno nájomníka.</span><span class="sxs-lookup"><span data-stu-id="c6f96-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="c6f96-110">Ak pracovný deň – nájomník – meno chýba, zlyhá overenie pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="c6f96-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="c6f96-111">Ak konfigurujete integráciu s nájomníkom vykonávania pracovného dňa, zaznamenajte si plánované prestoje v pracovnom čase nájomníka.</span><span class="sxs-lookup"><span data-stu-id="c6f96-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="c6f96-112">Pracovný deň naplánoval časový úsek pre svojich nájomníkov v priebehu víkendov (zvyčajne z piatku večer do soboty ráno) a zlyhanie pripojenia počas tohto časového obdobia je známy problém, ktorý sa automaticky vyrieši, hneď ako budú nájomníki implementácie naspäť online.</span><span class="sxs-lookup"><span data-stu-id="c6f96-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="c6f96-113">V zriedkavých prípadoch sa môže táto chyba Zobraziť aj v prípade, že sa heslo používateľa systému integrácie zmenilo z dôvodu obnovenia nájomníka alebo ak je konto v stave uzamknutia alebo skončenia platnosti.</span><span class="sxs-lookup"><span data-stu-id="c6f96-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="c6f96-114">Skontrolujte stav používateľa systému integrácie s správcom pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="c6f96-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="c6f96-115">Ďalšie informácie o konfigurácii pracovného dňa na automatické poskytovanie informácií nájdete v téme [kurz: Konfigurácia pracovného dňa na automatické poskytovanie používateľov](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="c6f96-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
