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
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509003"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="81a43-102">Denníky auditu odstránených e-mailových správ</span><span class="sxs-lookup"><span data-stu-id="81a43-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="81a43-103">Od januára 2019, Microsoft predvolene zapína zapisovanie do denníka auditu poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="81a43-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="81a43-104">Ak chcete skontrolovať udalosti správy pre konkrétneho používateľa, musíte manuálne povoliť akcie odstránenia na auditovanie.</span><span class="sxs-lookup"><span data-stu-id="81a43-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="81a43-105">Ak poštovej schránky auditu zapisovania do denníka je už povolená pre vašu organizáciu alebo pre konkrétneho používateľa, postupujte podľa krokov uvedených nižšie.</span><span class="sxs-lookup"><span data-stu-id="81a43-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="81a43-106">Prihláste sa do [Centra súladu zabezpečenia & microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="81a43-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="81a43-107">Kliknite na **položku Vyhľadávanie a vyšetrovanie** a vyberte položku **Hľadať denník auditu**.</span><span class="sxs-lookup"><span data-stu-id="81a43-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="81a43-108">Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Koncový dátum.**</span><span class="sxs-lookup"><span data-stu-id="81a43-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="81a43-109">Zadajte meno používateľa, ktorého chcete preskúmať (používateľa, ktorý položky odstránil).</span><span class="sxs-lookup"><span data-stu-id="81a43-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="81a43-110">V poli **Aktivity** vyberte položku **Odstránené správy z priečinka Odstránené položky** a **Premiestniť správy do priečinka Odstránené položky**.</span><span class="sxs-lookup"><span data-stu-id="81a43-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="81a43-111">Kliknite na tlačidlo **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="81a43-111">Click **Search**.</span></span>

<span data-ttu-id="81a43-112">Vo výsledkoch vyberte záznam auditu.</span><span class="sxs-lookup"><span data-stu-id="81a43-112">In the results, select an audit record.</span></span> <span data-ttu-id="81a43-113">V rozbaľovacom zozname podrobností kliknite na položku **Ďalšie informácie**.</span><span class="sxs-lookup"><span data-stu-id="81a43-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="81a43-114">Ďalšie informácie o odstránenej položke (napríklad predmet a umiestnenie položky pri jej odstránení) sa zobrazia v poli **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="81a43-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="81a43-115">Vlastnosť **ClientInfoString** sa zobrazí, ak sa odstránenie vyskytlo v programe Outlook, Outlook na webe (predtým známa ako aplikácia Outlook Web App) alebo v akomkoľvek inom zariadení.</span><span class="sxs-lookup"><span data-stu-id="81a43-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="81a43-116">Ďalšie informácie sa nachádzajú v téme [Určenie osôb, ktoré nastavia preposielanie e-mailov pre poštovú schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="81a43-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="81a43-117">**Poznámka:** Odstránené položky nie je možné načítať pomocou funkcie denníka auditu.</span><span class="sxs-lookup"><span data-stu-id="81a43-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="81a43-118">Informácie o načítanie odstránených správ v Outlooku na webe nájdete v téme [Obnovenie odstránených položiek v aplikácii Aplikácia Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="81a43-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
