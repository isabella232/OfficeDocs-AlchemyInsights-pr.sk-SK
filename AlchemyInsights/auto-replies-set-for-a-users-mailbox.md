---
title: Nastavenie automatických odpovedí pre poštovú schránku
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820949"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="cfbd6-102">Nastavenie automatických odpovedí pre poštovú schránku používateľa</span><span class="sxs-lookup"><span data-stu-id="cfbd6-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="cfbd6-103">**Metóda 1**</span><span class="sxs-lookup"><span data-stu-id="cfbd6-103">**Method 1**</span></span>

1. <span data-ttu-id="cfbd6-104">Prihláste sa na portáli služby Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cfbd6-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="cfbd6-105">Prejdite na položky **Používatelia > Aktívni používatelia** (alebo **Skupiny > Zdieľané poštové schránky**, ak to nastavujete v zdieľanej poštovej schránke).</span><span class="sxs-lookup"><span data-stu-id="cfbd6-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="cfbd6-106">Vyberte používateľa, ktorý má poštovú schránku servera Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="cfbd6-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="cfbd6-107">V rozbaľovacej ponuke na pravej strane prejdite na položky **Nastavenia pošty > Automatické odpovede** (ak ide o zdieľanú poštovú schránku, stačí kliknúť na položku **Automatické odpovede** v rozbaľovacej ponuke).</span><span class="sxs-lookup"><span data-stu-id="cfbd6-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="cfbd6-108">**Metóda 2**</span><span class="sxs-lookup"><span data-stu-id="cfbd6-108">**Method 2**</span></span>

1. <span data-ttu-id="cfbd6-109">Prihláste sa na portáli pre správcov služby Microsoft 365 pomocou prihlasovacích údajov správcu.</span><span class="sxs-lookup"><span data-stu-id="cfbd6-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="cfbd6-110">Rozbaľte ponuku **Centrá spravovania** a potom kliknite na položku **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="cfbd6-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="cfbd6-111">Kliknite na obrázok v pravom hornom rohu, kliknite na položku **Iný používateľ** a potom vyberte poštovú schránku používateľa, ktorú chcete zmeniť.</span><span class="sxs-lookup"><span data-stu-id="cfbd6-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="cfbd6-112">Na ľavej strane vyberte položku **Možnosti**, kliknite na položku **Organizovať e-mail** a potom kliknite na položku **Automatické odpovede.**</span><span class="sxs-lookup"><span data-stu-id="cfbd6-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="cfbd6-113">**Metóda 3**</span><span class="sxs-lookup"><span data-stu-id="cfbd6-113">**Method 3**</span></span>

<span data-ttu-id="cfbd6-114">Spustite nasledujúcu rutinu typu cmdlet v prostredí Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="cfbd6-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="cfbd6-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="cfbd6-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="cfbd6-116">Ďalšie informácie o tejto rutine typu cmdlet nájdete v téme [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="cfbd6-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
