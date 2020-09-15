---
title: Chýbajúce e-maily v karanténe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673729"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="bdcd0-102">Chýbajúce e-maily v karanténe</span><span class="sxs-lookup"><span data-stu-id="bdcd0-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="bdcd0-103">Správcovia môžu [tieto správy zobrazovať, uvoľňovať alebo odstraňovať.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="bdcd0-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="bdcd0-104">Ak chcete otvoriť centrum zabezpečenia & dodržiavania súladu, prejdite na [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="bdcd0-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="bdcd0-105">Ak chcete otvoriť stránku karantény priamo, prejdite na položku [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="bdcd0-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="bdcd0-106">Môžete vyhľadávať podľa nasledujúcich hodnôt:</span><span class="sxs-lookup"><span data-stu-id="bdcd0-106">You can search by the following values:</span></span>  

- <span data-ttu-id="bdcd0-107">**ID správy**: globálny jedinečný identifikátor správy.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="bdcd0-108">Ak v zozname vyberiete správu, na zobrazenej table s **podrobnosťami** sa zobrazí hodnota **ID správy** .</span><span class="sxs-lookup"><span data-stu-id="bdcd0-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="bdcd0-109">Správcovia môžu použiť [sledovanie](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) správ na vyhľadanie správ a príslušných hodnôt identifikácie správ.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="bdcd0-110">**E-mailová adresa odosielateľa**: e-mailová adresa jedného odosielateľa.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="bdcd0-111">**E-mailová adresa príjemcu**: e-mailová adresa jedného príjemcu.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="bdcd0-112">**Predmet**: použite celý predmet správy.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="bdcd0-113">Vyhľadávanie nerozlišuje veľké a malé písmená.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="bdcd0-114">Po zadaní kritérií vyhľadávania kliknite na položku Obnoviť ![ tlačidlo ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **obnoviť** a výsledky sa filtrujú.  </span><span class="sxs-lookup"><span data-stu-id="bdcd0-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="bdcd0-115">Rutiny typu cmdlet, ktoré používate na zobrazenie a spravovanie správ a súborov v karanténe, sú:</span><span class="sxs-lookup"><span data-stu-id="bdcd0-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="bdcd0-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="bdcd0-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="bdcd0-117">Export – QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="bdcd0-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="bdcd0-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="bdcd0-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="bdcd0-119">[Ukážka – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Táto rutina typu cmdlet je len pre správy, nie malvérové súbory z ATP pre SharePoint Online, OneDrive for Business alebo teams.</span><span class="sxs-lookup"><span data-stu-id="bdcd0-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="bdcd0-120">Vydanie – QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="bdcd0-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)