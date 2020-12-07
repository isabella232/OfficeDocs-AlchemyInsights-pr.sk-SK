---
title: Ikona kalendára sa nezobrazuje v klientovi Microsoft teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583926"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="54d87-102">Ikona kalendára sa nezobrazuje v klientovi Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="54d87-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="54d87-103">Karta **Kalendár** v aplikácii teams vyžaduje prístup k poštovej schránke programu Exchange prostredníctvom webových služieb Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="54d87-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="54d87-104">Poštová schránka Exchange môže byť online alebo lokálne.</span><span class="sxs-lookup"><span data-stu-id="54d87-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="54d87-105">V prípade online používateľov, ktorí nezobrazujú kartu **Kalendár** , skontrolujte, či majú [licenciu na poštovú schránku služby Exchange Online a či je poštová schránka povolená](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="54d87-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="54d87-106">Ak sú vaši používatelia doma lokálne, musíte potvrdiť, že vaša hybridná konfigurácia je zdravá.</span><span class="sxs-lookup"><span data-stu-id="54d87-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="54d87-107">Ak chcete riešiť problémy, použite [Sprievodcu hybridnou konfiguráciou](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="54d87-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="54d87-108">Upozorňujeme, že [aplikácia Teams vyžaduje Exchange 2016 CU3 alebo novší](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="54d87-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="54d87-109">Ďalšie informácie a kroky na riešenie problémov nájdete v téme [Riešenie problémov s interakciou aplikácie Microsoft teams a Exchange servera](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="54d87-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
