---
title: Identifikujte externé posielanie e-mailov v poštových schránkach v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716475"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="0a336-102">Identifikovať, keď externý e-mail presmerovanie je nakonfigurovaný na poštové schránky</span><span class="sxs-lookup"><span data-stu-id="0a336-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="0a336-103">Keď používateľ Microsoft 365 nakonfiguruje externý e-mail forwarding na poštovú schránku, aktivita je auditovaný ako súčasť rutiny cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="0a336-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="0a336-104">Aktivitu môžete vidieť pomocou vyhľadávania denníka auditu v centre zabezpečenia & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="0a336-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="0a336-105">Prihláste sa do [Microsoft 365 Security & centrum súladu](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="0a336-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="0a336-106">Prejdite na stránku vyhľadávania**denníka auditu** **vyhľadávania** > .</span><span class="sxs-lookup"><span data-stu-id="0a336-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="0a336-107">Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Dátum ukončenia** .</span><span class="sxs-lookup"><span data-stu-id="0a336-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="0a336-108">Nie je potrebné zadať používateľské meno.</span><span class="sxs-lookup"><span data-stu-id="0a336-108">You don't need to specify a username.</span></span> <span data-ttu-id="0a336-109">Overte, či je pole **aktivity** nastavené na **zobrazenie výsledkov pre všetky aktivity**.</span><span class="sxs-lookup"><span data-stu-id="0a336-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="0a336-110">Kliknite na tlačidlo **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="0a336-110">Click **Search**.</span></span>

<span data-ttu-id="0a336-111">Vo výsledkoch kliknite na položku **výsledky filtrovania** a zadajte do poľa Filter aktivity pole **nastaviť poštovú schránku** .</span><span class="sxs-lookup"><span data-stu-id="0a336-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="0a336-112">Vo výsledkoch vyberte záznam auditu.</span><span class="sxs-lookup"><span data-stu-id="0a336-112">Select an audit record in the results.</span></span> <span data-ttu-id="0a336-113">V rozbaľovacom zozname **Podrobnosti** kliknite na položku **Ďalšie informácie**.</span><span class="sxs-lookup"><span data-stu-id="0a336-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="0a336-114">Ak chcete zistiť, či aktivita súvisí s posielaním e-mailov, musíte sa pozrieť na Podrobnosti každého záznamu auditu.</span><span class="sxs-lookup"><span data-stu-id="0a336-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="0a336-115">**ObjectID**: alias hodnota poštovej schránky, ktorá bola zmenená.</span><span class="sxs-lookup"><span data-stu-id="0a336-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="0a336-116">**Parametre**: _ForwardingSMTPAddress_ označuje cieľovú e-mailovú adresu.</span><span class="sxs-lookup"><span data-stu-id="0a336-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="0a336-117">**Userid**: používateľ, ktorý nakonfiguroval presmerovanie e-mailov na poštovú schránku v poli **objectID** .</span><span class="sxs-lookup"><span data-stu-id="0a336-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="0a336-118">Ďalšie informácie nájdete v téme [určenie, kto nastaviť presmerovanie e-mailov pre poštovú schránku](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="0a336-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
