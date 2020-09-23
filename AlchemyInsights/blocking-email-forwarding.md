---
title: 726 blokovanie preposielania e-mailov
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219870"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="9704c-102">Blokovanie alebo odblokovanie preposielania e-mailov</span><span class="sxs-lookup"><span data-stu-id="9704c-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="9704c-103">Ak chcete zapnúť alebo vypnúť presmerovanie e-mailov pre konkrétnu poštovú schránku, prečítajte si tému [Konfigurácia preposielania](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)</span><span class="sxs-lookup"><span data-stu-id="9704c-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="9704c-104">Na úrovni nájomníka sa kontrola externého preposielania uskutočňuje pomocou odchádzajúcej politiky ochrany pred nevyžiadanou poštou.</span><span class="sxs-lookup"><span data-stu-id="9704c-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="9704c-105">Ak je nastavená na možnosť vypnutá alebo automatická, môže blokovať preposielanie e-mailov s odmietnutým prístupom "550 5.7.520, vaša organizácia nepovoľuje externé preposielanie".</span><span class="sxs-lookup"><span data-stu-id="9704c-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="9704c-106">Následne, ak bolo preposielanie nastavené na možnosť blokované, znamená to chybu, ktorú budú používatelia zobrazovať.</span><span class="sxs-lookup"><span data-stu-id="9704c-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="9704c-107">Ak je presmerovanie zablokované, skontrolujte, či je politika nakonfigurovaná na povolenie externého preposielania.</span><span class="sxs-lookup"><span data-stu-id="9704c-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="9704c-108">Odchádzajúca politika filtrovania nevyžiadanej pošty môžete skontrolovať v centre zabezpečenia a dodržiavania súladu alebo spustením príkazu Get-HostedOutboundSpamFilterPolicy | FL Name, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="9704c-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="9704c-109">Ak chcete nastaviť blokovanie automaticky preposielaných údajov, rovnaký príkaz vám oznámi stav politiky.</span><span class="sxs-lookup"><span data-stu-id="9704c-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="9704c-110">Poznámka: odporúča sa ponechať externé automatické preposielanie vypnuté v predvolenej politike filtra odchádzajúcich nevyžiadanej pošty a povoliť ho len používateľom, ktorí potrebujú externé preposielanie, a to vytvorením vlastnej politiky pre týchto používateľov.</span><span class="sxs-lookup"><span data-stu-id="9704c-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="9704c-111">Ďalšie informácie nájdete v téme [Konfigurácia externého preposielania e-mailov v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="9704c-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>