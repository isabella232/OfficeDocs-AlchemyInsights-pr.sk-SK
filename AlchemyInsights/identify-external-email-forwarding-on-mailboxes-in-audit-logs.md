---
title: Identifikácia externého preposielania e-mailov poštových schránok v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696312"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="54075-102">Určenie, kedy je externé presmerovanie e-mailov nakonfigurované v poštových schránkach</span><span class="sxs-lookup"><span data-stu-id="54075-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="54075-103">Keď používateľ programu Microsoft 365 nakonfiguruje externé preposielanie e-mailov v poštovej schránke, aktivita sa Audituje ako súčasť rutiny typu cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="54075-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="54075-104">Aktivitu môžete zobraziť pomocou vyhľadávania denníkov auditu v centre zabezpečenia & dodržiavania súladu.</span><span class="sxs-lookup"><span data-stu-id="54075-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="54075-105">Prihláste sa do [Centra zabezpečenia dodržiavania súladu so službou Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="54075-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="54075-106">Prejdite na stránku **Search**  >  **vyhľadávania denníka auditu** vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="54075-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="54075-107">V poliach **Počiatočný** dátum a **Koncový dátum** vyberte rozsah dátumov.</span><span class="sxs-lookup"><span data-stu-id="54075-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="54075-108">Nemusíte špecifikovať meno používateľa.</span><span class="sxs-lookup"><span data-stu-id="54075-108">You don't need to specify a username.</span></span> <span data-ttu-id="54075-109">Overte, či je pole **aktivity** nastavené na možnosť **Zobraziť výsledky pre všetky aktivity**.</span><span class="sxs-lookup"><span data-stu-id="54075-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="54075-110">Kliknite na položku **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="54075-110">Click **Search**.</span></span>

<span data-ttu-id="54075-111">Vo výsledkoch kliknite na položku **filtrovať výsledky** a do poľa Filter aktivity zadajte výraz **množina poštových schránok** .</span><span class="sxs-lookup"><span data-stu-id="54075-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="54075-112">Vo výsledkoch vyberte záznam auditu.</span><span class="sxs-lookup"><span data-stu-id="54075-112">Select an audit record in the results.</span></span> <span data-ttu-id="54075-113">V rozbaľovacom zozname **Podrobnosti** kliknite na položku **Ďalšie informácie**.</span><span class="sxs-lookup"><span data-stu-id="54075-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="54075-114">Ak chcete zistiť, či sa aktivita týka preposielania e-mailov, musíte si pozrieť podrobnosti o každom zázname auditu.</span><span class="sxs-lookup"><span data-stu-id="54075-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="54075-115">**ObjectID**: hodnota aliasu v poštovej schránke, ktorá bola upravená.</span><span class="sxs-lookup"><span data-stu-id="54075-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="54075-116">**Parametre**: _ForwardingSMTPAddress_ označuje cieľovú e-mailovú adresu.</span><span class="sxs-lookup"><span data-stu-id="54075-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="54075-117">**Userid**: používateľ, ktorý nakonfiguroval preposielanie e-mailov v poštovej schránke v poli **objectID** .</span><span class="sxs-lookup"><span data-stu-id="54075-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="54075-118">Ďalšie informácie nájdete v téme [Určenie používateľov, ktorí nastavujú preposielanie e-mailov pre poštovú schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="54075-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
