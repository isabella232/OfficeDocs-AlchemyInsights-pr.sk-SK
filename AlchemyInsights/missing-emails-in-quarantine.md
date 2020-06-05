---
title: Chýbajúce e-maily v karanténe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569559"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="5b39d-102">Chýbajúce e-maily v karanténe"</span><span class="sxs-lookup"><span data-stu-id="5b39d-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="5b39d-103">Správcovia môžu [tieto správy zobraziť, uvoľniť alebo odstrániť.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="5b39d-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="5b39d-104">Ak chcete otvoriť Centrum zabezpečenia & súladu, prejdite na položku [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="5b39d-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="5b39d-105">Ak chcete otvoriť stránku Karanténa priamo, prejdite na položku [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="5b39d-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="5b39d-106">Môžete vyhľadávať podľa nasledujúcich hodnôt:</span><span class="sxs-lookup"><span data-stu-id="5b39d-106">You can search by the following values:</span></span>  

- <span data-ttu-id="5b39d-107">**Identifikácia správy:** Globálne jedinečný identifikátor správy.</span><span class="sxs-lookup"><span data-stu-id="5b39d-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="5b39d-108">Ak vyberiete správu v zozname, hodnota **Id správy** sa zobrazí na table **Podrobnosti** rozbaľovacieho zoznamu, ktorá sa zobrazí.</span><span class="sxs-lookup"><span data-stu-id="5b39d-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="5b39d-109">Správcovia môžu použiť [sledovanie správ](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) na vyhľadanie správ a zodpovedajúcich hodnôt identifikácie správy.</span><span class="sxs-lookup"><span data-stu-id="5b39d-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="5b39d-110">**E-mailová adresa odosielateľa**: E-mailová adresa jedného odosielateľa.</span><span class="sxs-lookup"><span data-stu-id="5b39d-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="5b39d-111">**E-mailová adresa príjemcu:** e-mailová adresa jedného príjemcu.</span><span class="sxs-lookup"><span data-stu-id="5b39d-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="5b39d-112">**Predmet**: Použite celý predmet správy.</span><span class="sxs-lookup"><span data-stu-id="5b39d-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="5b39d-113">Pri vyhľadávaní sa nerozlišujú veľké a malé písmená.</span><span class="sxs-lookup"><span data-stu-id="5b39d-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="5b39d-114">Po zadaní kritérií vyhľadávania kliknutím na ![ tlačidlo Obnoviť kliknite na tlačidlo ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Obnoviť** a výsledky môžete filtrovať.  </span><span class="sxs-lookup"><span data-stu-id="5b39d-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="5b39d-115">Rutiny cmdlet, ktoré používate na zobrazenie a správu správ a súborov v karanténe, sú:</span><span class="sxs-lookup"><span data-stu-id="5b39d-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="5b39d-116">Odstrániť karanténuMessage</span><span class="sxs-lookup"><span data-stu-id="5b39d-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="5b39d-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="5b39d-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="5b39d-118">Získajte karanténuMessage</span><span class="sxs-lookup"><span data-stu-id="5b39d-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="5b39d-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Všimnite si, že táto rutina cmdlet je len pre správy, nie malware súbory z ATP pre SharePoint Online, OneDrive pre podniky alebo tímy.</span><span class="sxs-lookup"><span data-stu-id="5b39d-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="5b39d-120">Správa o vydaní karantény</span><span class="sxs-lookup"><span data-stu-id="5b39d-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)