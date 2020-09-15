---
title: Identifikácia odstraňovania udalostí správy v denníkoch auditu
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696528"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="c28bc-102">Denníky auditu odstránených e-mailových správ</span><span class="sxs-lookup"><span data-stu-id="c28bc-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="c28bc-103">Od januára 2019 spoločnosť Microsoft zapne zapisovanie do denníka auditu poštovej schránky na základe predvoleného nastavenia.</span><span class="sxs-lookup"><span data-stu-id="c28bc-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="c28bc-104">Ak v opačnom prípade chcete skontrolovať odstránenie udalostí správy pre konkrétneho používateľa, musíte manuálne povoliť akcie odstránenia na auditovanie.</span><span class="sxs-lookup"><span data-stu-id="c28bc-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="c28bc-105">Ak je zapisovanie do denníka auditu poštovej schránky pre vašu organizáciu alebo konkrétneho používateľa už zapnuté, postupujte podľa nižšie uvedených krokov.</span><span class="sxs-lookup"><span data-stu-id="c28bc-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="c28bc-106">Prihláste sa do [Centra zabezpečenia dodržiavania súladu so službou Microsoft 365 Security &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="c28bc-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="c28bc-107">Kliknite na položku **vyhľadávanie a šetrenie** a vyberte položku **vyhľadávanie denníkov auditu**.</span><span class="sxs-lookup"><span data-stu-id="c28bc-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="c28bc-108">V poliach **Počiatočný** dátum a **Koncový dátum** vyberte rozsah dátumov.</span><span class="sxs-lookup"><span data-stu-id="c28bc-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c28bc-109">Zadajte meno používateľa, ktoré chcete preskúmať (používateľ, ktorý odstránil položky).</span><span class="sxs-lookup"><span data-stu-id="c28bc-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="c28bc-110">V poli **aktivity** vyberte položku **odstránené správy z priečinka Odstránené položky** a **premiestnené správy do priečinka Odstránené položky**.</span><span class="sxs-lookup"><span data-stu-id="c28bc-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="c28bc-111">Kliknite na položku **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="c28bc-111">Click **Search**.</span></span>

<span data-ttu-id="c28bc-112">Vo výsledkoch vyberte záznam auditu.</span><span class="sxs-lookup"><span data-stu-id="c28bc-112">In the results, select an audit record.</span></span> <span data-ttu-id="c28bc-113">V rozbaľovacom zozname Podrobnosti kliknite na položku **Ďalšie informácie**.</span><span class="sxs-lookup"><span data-stu-id="c28bc-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="c28bc-114">Ďalšie informácie o odstránenej položke (napríklad riadok predmetu a umiestnenie položky pri odstránení) sa zobrazia v poli **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="c28bc-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="c28bc-115">Vlastnosť **ClientInfoString** sa zobrazí, ak sa v Outlooku, Outlooku na webe (predtým známy ako Outlook Web App) alebo v ľubovoľnom inom zariadení zobrazuje odstránenie.</span><span class="sxs-lookup"><span data-stu-id="c28bc-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="c28bc-116">Ďalšie informácie nájdete v téme [Určenie používateľov, ktorí nastavujú preposielanie e-mailov pre poštovú schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="c28bc-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="c28bc-117">**Poznámka**: odstránené položky nie je možné načítať pomocou funkcie denník auditu.</span><span class="sxs-lookup"><span data-stu-id="c28bc-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="c28bc-118">Ak chcete obnoviť odstránené správy v Outlooku na webe, prečítajte si tému [Obnovenie odstránených položiek v aplikácii Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="c28bc-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
