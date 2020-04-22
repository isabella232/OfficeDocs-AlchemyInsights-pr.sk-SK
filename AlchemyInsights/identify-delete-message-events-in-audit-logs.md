---
title: Identifikácia udalostí odstránenia správy v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716511"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="17168-102">Denníky auditu pre odstránené e-mailové správy</span><span class="sxs-lookup"><span data-stu-id="17168-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="17168-103">Od januára 2019, Microsoft je Zapnutie poštovej schránky auditu zapisovania do denníka v predvolenom nastavení.</span><span class="sxs-lookup"><span data-stu-id="17168-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="17168-104">V opačnom prípade môžete skontrolovať odstránenie udalostí správy pre konkrétneho používateľa, musíte manuálne povoliť akcie odstránenia pre auditovanie.</span><span class="sxs-lookup"><span data-stu-id="17168-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="17168-105">Ak poštovej schránky auditu zapisovania je už povolená pre vašu organizáciu alebo pre konkrétneho používateľa, postupujte podľa nasledujúcich krokov.</span><span class="sxs-lookup"><span data-stu-id="17168-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="17168-106">Prihláste sa do [Microsoft 365 zabezpečenia & Compliance Center](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="17168-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="17168-107">Kliknite na položku **vyhľadávanie a vyšetrovanie** a vyberte položku **vyhľadávanie denníkov auditu**.</span><span class="sxs-lookup"><span data-stu-id="17168-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="17168-108">Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Dátum ukončenia** .</span><span class="sxs-lookup"><span data-stu-id="17168-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="17168-109">Zadajte používateľské meno používateľa, ktorý chcete zistiť (používateľ, ktorý odstránil položky).</span><span class="sxs-lookup"><span data-stu-id="17168-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="17168-110">V poli **aktivity** vyberte položku **odstránené správy z priečinka Odstránené položky** a **premiestnili sa správy do priečinka Odstránené položky**.</span><span class="sxs-lookup"><span data-stu-id="17168-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="17168-111">Kliknite na tlačidlo **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="17168-111">Click **Search**.</span></span>

<span data-ttu-id="17168-112">Vo výsledkoch vyberte záznam auditu.</span><span class="sxs-lookup"><span data-stu-id="17168-112">In the results, select an audit record.</span></span> <span data-ttu-id="17168-113">V rozbaľovacom zozname Podrobnosti kliknite na položku **Ďalšie informácie**.</span><span class="sxs-lookup"><span data-stu-id="17168-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="17168-114">Ďalšie informácie o odstránenej položke (napríklad riadok predmetu a umiestnenie položky pri jej odstránení) sa zobrazia v poli **Affecteditems** .</span><span class="sxs-lookup"><span data-stu-id="17168-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="17168-115">Vlastnosť **Clientinfostring** sa zobrazí, ak sa odstránenie vyskytlo v programe Outlook, Outlook na webe (predtým označované ako aplikácia Outlook Web App) alebo v akomkoľvek inom zariadení.</span><span class="sxs-lookup"><span data-stu-id="17168-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="17168-116">Ďalšie informácie nájdete v téme [určenie, kto nastaviť presmerovanie e-mailov pre poštovú schránku](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="17168-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="17168-117">**Poznámka**: odstránené položky nie je možné načítať pomocou funkcie denník auditu.</span><span class="sxs-lookup"><span data-stu-id="17168-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="17168-118">Ak chcete obnoviť odstránené správy v programe Outlook na webe, pozrite si ďalšie informácie [v téme Obnovenie odstránených položiek v aplikácii Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="17168-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
