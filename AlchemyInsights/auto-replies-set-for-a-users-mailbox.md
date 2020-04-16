---
title: Nastavenie automatických odpovedí pre poštovú schránku
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
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509516"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="c9849-102">Nastavenie automatických odpovedí pre poštovú schránku používateľa</span><span class="sxs-lookup"><span data-stu-id="c9849-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="c9849-103">**Metóda 1**</span><span class="sxs-lookup"><span data-stu-id="c9849-103">**Method 1**</span></span>

1. <span data-ttu-id="c9849-104">Prihláste sa na portáli služieb Office 365.</span><span class="sxs-lookup"><span data-stu-id="c9849-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="c9849-105">Prejdite na položky **Používatelia > Aktívni používatelia** (alebo **Skupiny > Zdieľané poštové schránky**, ak to nastavujete v zdieľanej poštovej schránke).</span><span class="sxs-lookup"><span data-stu-id="c9849-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="c9849-106">Vyberte používateľa, ktorý má poštovú schránku servera Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9849-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="c9849-107">V rozbaľovacej ponuke na pravej strane prejdite na položky **Nastavenia pošty > Automatické odpovede** (ak ide o zdieľanú poštovú schránku, stačí kliknúť na položku **Automatické odpovede** v rozbaľovacej ponuke).</span><span class="sxs-lookup"><span data-stu-id="c9849-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="c9849-108">**Metóda 2**</span><span class="sxs-lookup"><span data-stu-id="c9849-108">**Method 2**</span></span>

1. <span data-ttu-id="c9849-109">Prihláste sa na portáli pre správcov služieb Office 365 pomocou prihlasovacích údajov správcu.</span><span class="sxs-lookup"><span data-stu-id="c9849-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="c9849-110">Rozbaľte ponuku **Centrá spravovania** a potom kliknite na položku **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c9849-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="c9849-111">Kliknite na obrázok v pravom hornom rohu, kliknite na položku **Iný používateľ** a potom vyberte poštovú schránku používateľa, ktorú chcete zmeniť.</span><span class="sxs-lookup"><span data-stu-id="c9849-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="c9849-112">Na ľavej strane vyberte položku **Možnosti**, kliknite na položku **Organizovať e-mail** a potom kliknite na položku **Automatické odpovede.**</span><span class="sxs-lookup"><span data-stu-id="c9849-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="c9849-113">**Metóda 3**</span><span class="sxs-lookup"><span data-stu-id="c9849-113">**Method 3**</span></span>

<span data-ttu-id="c9849-114">Spustite nasledujúcu rutinu typu cmdlet v prostredí Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="c9849-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="c9849-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="c9849-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="c9849-116">Ďalšie informácie o tejto rutine typu cmdlet nájdete v téme [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="c9849-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
