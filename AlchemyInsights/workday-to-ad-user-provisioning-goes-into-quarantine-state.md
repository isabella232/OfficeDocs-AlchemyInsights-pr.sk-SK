---
title: Pracovný deň na poskytovanie AD používateľov ide do stavu karantény
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482903"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="ca7c1-102">Pracovný deň na poskytovanie AD používateľov ide do stavu karantény</span><span class="sxs-lookup"><span data-stu-id="ca7c1-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="ca7c1-103">**Pracovný deň na poskytovanie AD používateľov prejde do stavu karantény a v službe AD sa nevytvára žiaden používateľ**</span><span class="sxs-lookup"><span data-stu-id="ca7c1-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="ca7c1-104">Pracovný deň s poskytnutím úlohy AD user v karanténe a denníky auditu zobrazujú udalosti zlyhania exportu s chybovým hlásením **chyba: OperationsError-SvcErr: Vyskytla sa chyba operácie. Pre adresárovú službu nebol nakonfigurovaný žiadny nadriadený odkaz. Adresárová služba preto nedokáže vydať odporúčania na objekty mimo tohto lesa**.</span><span class="sxs-lookup"><span data-stu-id="ca7c1-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="ca7c1-105">Táto chyba sa zvyčajne zobrazuje v prípade, že kontajner služby Active Directory nie je nastavený správne alebo ak sa vyskytnú problémy s priradením výrazov, ktoré sa používajú pre **parentDistinguishedName**.</span><span class="sxs-lookup"><span data-stu-id="ca7c1-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="ca7c1-106">Skontrolujte predvolený parameter OU pre **nových používateľov** pre preklepy.</span><span class="sxs-lookup"><span data-stu-id="ca7c1-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="ca7c1-107">Uistite sa, že určitá OU už v REKLAMe existuje.</span><span class="sxs-lookup"><span data-stu-id="ca7c1-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="ca7c1-108">Ak v priradení atribútov používate **parentDistinguishedName** , uistite sa, že sa vždy vyhodnotí v rámci reklamnej domény známym kontajnerom.</span><span class="sxs-lookup"><span data-stu-id="ca7c1-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="ca7c1-109">Ak chcete zobraziť vygenerovanú hodnotu, pozrite si udalosť exportu v denníkoch auditu.</span><span class="sxs-lookup"><span data-stu-id="ca7c1-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="ca7c1-110">Ďalšie informácie o konfigurácii pracovného dňa na automatické poskytovanie informácií nájdete v téme [kurz: Konfigurácia pracovného dňa na automatické poskytovanie používateľov](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="ca7c1-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

