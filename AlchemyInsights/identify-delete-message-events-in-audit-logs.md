---
title: Identifikáciu odstrániť správu udalostí v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416724"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="84711-102">Denníky pre audit odstránených e-mailových správ</span><span class="sxs-lookup"><span data-stu-id="84711-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="84711-103">Od januára 2019, Microsoft je odbočka na poštovej schránky auditu zapisovania do denníka v predvolenom nastavení.</span><span class="sxs-lookup"><span data-stu-id="84711-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="84711-104">Inak, skontrolujte odstrániť hlásenie udalosti pre konkrétneho používateľa, musíte manuálne povoliť akcie delete pre auditovanie.</span><span class="sxs-lookup"><span data-stu-id="84711-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="84711-105">Ak poštová schránka pre audit sú už povolené pre organizáciu alebo pre konkrétneho používateľa, postupujte podľa nasledujúcich krokov.</span><span class="sxs-lookup"><span data-stu-id="84711-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="84711-106">Prihláste sa do [Centrum Office 365 zabezpečenia & súlad](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="84711-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="84711-107">Kliknite na položku **vyhľadávanie a vyšetrovanie** a vyberte **Vyhľadávanie denník auditu**.</span><span class="sxs-lookup"><span data-stu-id="84711-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="84711-108">Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Koncový dátum** .</span><span class="sxs-lookup"><span data-stu-id="84711-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="84711-109">Zadajte meno používateľa, ktorý chcete preskúmať (používateľa, ktorý odstránil položky).</span><span class="sxs-lookup"><span data-stu-id="84711-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="84711-110">V oblasti **aktivity** vyberte **odstránené správy z priečinka Odstránené položky** a **správy presunuté do priečinka Odstránené položky**.</span><span class="sxs-lookup"><span data-stu-id="84711-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="84711-111">Kliknite na tlačidlo **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="84711-111">Click **Search**.</span></span>

<span data-ttu-id="84711-112">V zozname výsledkov vyberte auditný záznam.</span><span class="sxs-lookup"><span data-stu-id="84711-112">In the results, select an audit record.</span></span> <span data-ttu-id="84711-113">V rozbaľovacie tlačidlo Podrobnosti, kliknite na **Viac informácií**.</span><span class="sxs-lookup"><span data-stu-id="84711-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="84711-114">Ďalšie informácie o odstránených položiek (napríklad, predmet a umiestnenie položky, keď sa odstránil) je zobrazené v poli **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="84711-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="84711-115">Vlastnosť **ClientInfoString** zobrazí, ak odstránenia sa vyskytla v programe Outlook, Outlook web (predtým označované ako aplikácie Outlook Web App) alebo akékoľvek iné zariadenie.</span><span class="sxs-lookup"><span data-stu-id="84711-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="84711-116">Pre viac informácií, pozri [určenie kto nastaviť preposielanie pre poštovú schránku](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="84711-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="84711-117">**Poznámka**: nemožno obnoviť odstránené položky pomocou audit log funkcie.</span><span class="sxs-lookup"><span data-stu-id="84711-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="84711-118">Obnoviť odstránené položky v programe Outlook na webe, nájdete v téme [Obnovenie odstránených položiek v aplikácii Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="84711-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
