---
title: Nastavenie automatických odpovedí pre poštovú schránku používateľa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506647"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="b194d-102">Nastavenie automatických odpovedí pre poštovú schránku používateľa</span><span class="sxs-lookup"><span data-stu-id="b194d-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="b194d-103">**Metóda 1**</span><span class="sxs-lookup"><span data-stu-id="b194d-103">**Method 1**</span></span>

1. <span data-ttu-id="b194d-104">Prihláste sa na portáli služieb Office 365.</span><span class="sxs-lookup"><span data-stu-id="b194d-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="b194d-105">Prejdite na položky **Používatelia > Aktívni používatelia** (alebo **Skupiny > Zdieľané poštové schránky**, ak to nastavujete v zdieľanej poštovej schránke).</span><span class="sxs-lookup"><span data-stu-id="b194d-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="b194d-106">Vyberte používateľa, ktorý má poštovú schránku servera Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="b194d-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="b194d-107">V rozbaľovacej ponuke na pravej strane prejdite na položky **Nastavenia pošty > Automatické odpovede** (ak ide o zdieľanú poštovú schránku, stačí kliknúť na položku **Automatické odpovede** v rozbaľovacej ponuke).</span><span class="sxs-lookup"><span data-stu-id="b194d-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="b194d-108">**Metóda 2**</span><span class="sxs-lookup"><span data-stu-id="b194d-108">**Method 2**</span></span>

1. <span data-ttu-id="b194d-109">Prihláste sa na portáli pre správcov služieb Office 365 pomocou prihlasovacích údajov správcu.</span><span class="sxs-lookup"><span data-stu-id="b194d-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="b194d-110">Rozbaľte ponuku **Centrá spravovania** a potom kliknite na položku **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b194d-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="b194d-111">Kliknite na obrázok v pravom hornom rohu, kliknite na položku **Iný používateľ** a potom vyberte poštovú schránku používateľa, ktorú chcete zmeniť.</span><span class="sxs-lookup"><span data-stu-id="b194d-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="b194d-112">Na ľavej strane vyberte položku **Možnosti**, kliknite na položku **Organizovať e-mail** a potom kliknite na položku **Automatické odpovede.**</span><span class="sxs-lookup"><span data-stu-id="b194d-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="b194d-113">**Metóda 3**</span><span class="sxs-lookup"><span data-stu-id="b194d-113">**Method 3**</span></span>

<span data-ttu-id="b194d-114">Spustite nasledujúcu rutinu typu cmdlet v prostredí Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="b194d-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="b194d-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="b194d-115">PowerShellCopy</span></span>

    Set-MailboxAutoReplyConfiguration

<span data-ttu-id="b194d-116">Ďalšie informácie o tejto rutine typu cmdlet nájdete v téme [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="b194d-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
