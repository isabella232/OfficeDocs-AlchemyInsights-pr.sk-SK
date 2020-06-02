---
title: Identifikácia externého posielania e-mailov ďalej v poštových schránkach v denníkoch auditu
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
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508967"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="27289-102">Identifikácia, keď je externé presmerovanie e-mailov nakonfigurované v poštových schránkach</span><span class="sxs-lookup"><span data-stu-id="27289-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="27289-103">Keď používateľ Microsoft 365 nakonfiguruje externé e-mail presmerovanie poštovej schránky, činnosť je auditovaný ako súčasť rutiny cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="27289-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="27289-104">Aktivitu môžete zobraziť pomocou vyhľadávania denníka auditu v Centre zabezpečenia & súladu.</span><span class="sxs-lookup"><span data-stu-id="27289-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="27289-105">Prihláste sa do Centra [& zabezpečenia spoločnosti Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="27289-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="27289-106">Prejdite na stránku **vyhľadávania**  >  **v denníku auditu.**</span><span class="sxs-lookup"><span data-stu-id="27289-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="27289-107">Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Koncový dátum.**</span><span class="sxs-lookup"><span data-stu-id="27289-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="27289-108">Nie je potrebné zadať meno používateľa.</span><span class="sxs-lookup"><span data-stu-id="27289-108">You don't need to specify a username.</span></span> <span data-ttu-id="27289-109">Skontrolujte, či je pole **Aktivity** nastavené na **možnosť Zobraziť výsledky pre všetky aktivity**.</span><span class="sxs-lookup"><span data-stu-id="27289-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="27289-110">Kliknite na tlačidlo **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="27289-110">Click **Search**.</span></span>

<span data-ttu-id="27289-111">Vo výsledkoch kliknite na **položku Filtrovať výsledky** a do poľa filter aktivity zadajte text **Nastaviť poštovú schránku.**</span><span class="sxs-lookup"><span data-stu-id="27289-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="27289-112">Vo výsledkoch vyberte záznam auditu.</span><span class="sxs-lookup"><span data-stu-id="27289-112">Select an audit record in the results.</span></span> <span data-ttu-id="27289-113">V rozbaľovacom zozname **Podrobnosti** kliknite na položku **Ďalšie informácie**.</span><span class="sxs-lookup"><span data-stu-id="27289-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="27289-114">Ak chcete zistiť, či aktivita súvisí s posielaním e-mailov ďalej, musíte sa pozrieť na podrobnosti každého záznamu auditu.</span><span class="sxs-lookup"><span data-stu-id="27289-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="27289-115">**ObjectId:** Hodnota aliasu poštovej schránky, ktorá bola upravená.</span><span class="sxs-lookup"><span data-stu-id="27289-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="27289-116">**Parametre**: _ForwardingSmtpAddress_ označuje cieľovú e-mailovú adresu.</span><span class="sxs-lookup"><span data-stu-id="27289-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="27289-117">**UserId:** Používateľ, ktorý nakonfiguroval e-mail presmerovanie v poštovej schránke v **objectid** pole.</span><span class="sxs-lookup"><span data-stu-id="27289-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="27289-118">Ďalšie informácie sa nachádzajú v téme [Určenie osôb, ktoré nastavia preposielanie e-mailov pre poštovú schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="27289-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
