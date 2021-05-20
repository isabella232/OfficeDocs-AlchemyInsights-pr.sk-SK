---
title: Chýbajúce e-maily v karanténe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539839"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="086e2-102">Chýbajúce e-maily v karanténe"</span><span class="sxs-lookup"><span data-stu-id="086e2-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="086e2-103">Správcovia [môžu tieto správy zobraziť, uvoľniť alebo odstrániť.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="086e2-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="086e2-104">Ak chcete otvoriť Centrum zabezpečenia & zabezpečenia, prejdite na položku [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="086e2-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="086e2-105">Ak chcete stránku karantény otvoriť priamo, prejdite do ponuky [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="086e2-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="086e2-106">Vyhľadávať môžete podľa nasledujúcich hodnôt:</span><span class="sxs-lookup"><span data-stu-id="086e2-106">You can search by the following values:</span></span>  

- <span data-ttu-id="086e2-107">**ID správy:** globálny jedinečný identifikátor správy.</span><span class="sxs-lookup"><span data-stu-id="086e2-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="086e2-108">Ak vyberiete správu v zozname, na  **zobrazenej**  table Podrobnosti sa  **zobrazí**  hodnota ID správy.</span><span class="sxs-lookup"><span data-stu-id="086e2-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="086e2-109">Správcovia môžu pomocou [sledovania správ](/microsoft-365/security/office-365-security/message-trace-scc) vyhľadať správy a ich zodpovedajúce hodnoty ID správy.</span><span class="sxs-lookup"><span data-stu-id="086e2-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="086e2-110">**E-mailová adresa** odosielateľa: E-mailová adresa jedného odosielateľa.</span><span class="sxs-lookup"><span data-stu-id="086e2-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="086e2-111">**E-mailová** adresa príjemcu: E-mailová adresa jedného príjemcu.</span><span class="sxs-lookup"><span data-stu-id="086e2-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="086e2-112">**Predmet**: Použite celý predmet správy.</span><span class="sxs-lookup"><span data-stu-id="086e2-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="086e2-113">Pri vyhľadávaní sa rozlišujú malé a veľké písmená.</span><span class="sxs-lookup"><span data-stu-id="086e2-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="086e2-114">Po zadaní kritérií vyhľadávania kliknite na tlačidlo Obnoviť a ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **vyfiltrujte** výsledky.</span><span class="sxs-lookup"><span data-stu-id="086e2-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="086e2-115">Rutiny typu cmdlet, ktoré používate na zobrazenie a spravovanie správ a súborov v karanténe, sú:</span><span class="sxs-lookup"><span data-stu-id="086e2-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="086e2-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="086e2-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="086e2-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="086e2-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="086e2-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="086e2-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="086e2-119">[Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Táto rutina typu cmdlet je len pre správy, nie pre malvérové súbory z programu Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive for Business alebo Teams.</span><span class="sxs-lookup"><span data-stu-id="086e2-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="086e2-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="086e2-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)