---
title: Určiť externé preposielanie na poštové schránky v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417226"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="e5db5-102">Identifikovať preposielanie externých e-mailov je nakonfigurovaný poštových schránok</span><span class="sxs-lookup"><span data-stu-id="e5db5-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="e5db5-103">Keď používateľ nakonfiguruje externé preposielanie na poštovú schránku, činnosť je audit ako súčasť rutiny cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="e5db5-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="e5db5-104">Môžete vidieť aktivitu pomocou vyhľadávanie denník auditu bezpečnosti & centrum súladu.</span><span class="sxs-lookup"><span data-stu-id="e5db5-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="e5db5-105">Prihláste sa do [Centrum Office 365 zabezpečenia & súlad](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="e5db5-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="e5db5-106">Kliknite na položku **vyhľadávanie a vyšetrovanie** a vyberte **Vyhľadávanie denník auditu**.</span><span class="sxs-lookup"><span data-stu-id="e5db5-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="e5db5-107">Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Koncový dátum** .</span><span class="sxs-lookup"><span data-stu-id="e5db5-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="e5db5-108">Nemusíte zadať meno používateľa.</span><span class="sxs-lookup"><span data-stu-id="e5db5-108">You don't need to specify a username.</span></span> <span data-ttu-id="e5db5-109">Overenie **činnosti** pole nastavené na **zobrazenie výsledkov pre všetky činnosti**.</span><span class="sxs-lookup"><span data-stu-id="e5db5-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="e5db5-110">Kliknite na tlačidlo **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="e5db5-110">Click **Search**.</span></span>

<span data-ttu-id="e5db5-111">Vo výsledkoch kliknite na položku **Filtrovať výsledky** a aktivity filtra poľa zadajte **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="e5db5-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="e5db5-112">Vyberte auditný záznam výsledkov.</span><span class="sxs-lookup"><span data-stu-id="e5db5-112">Select an audit record in the results.</span></span> <span data-ttu-id="e5db5-113">Rozbaľovacie tlačidlo **Podrobnosti** , kliknite na **viac informácií**.</span><span class="sxs-lookup"><span data-stu-id="e5db5-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="e5db5-114">Musíte sa pozrieť na detaily každého záznamu auditu na určenie, či činnosť súvisí preposielanie e-mailov.</span><span class="sxs-lookup"><span data-stu-id="e5db5-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="e5db5-115">**ObjectId**: hodnotu alias poštovej schránky, ktorá bola upravená.</span><span class="sxs-lookup"><span data-stu-id="e5db5-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="e5db5-116">**Parametre**: _ForwardingSmtpAddress_ označuje cieľovú e-mailovú adresu.</span><span class="sxs-lookup"><span data-stu-id="e5db5-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="e5db5-117">**ID užívateľa**: používateľ nakonfigurovaný preposielanie e-mailov v poštovej schránke v poli **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="e5db5-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="e5db5-118">Pre viac informácií, pozri [určenie kto nastaviť preposielanie pre poštovú schránku](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="e5db5-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
