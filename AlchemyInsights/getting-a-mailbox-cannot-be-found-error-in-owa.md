---
title: 126 Nepodarilo sa v aplikácii OWA nájsť chybu o získaní poštovej schránky?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426677"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="f4151-102">Zobrazuje sa vám v Outlooku na webe chyba o tom, že sa poštová schránka nenašiel?</span><span class="sxs-lookup"><span data-stu-id="f4151-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="f4151-103">Ak používate Outlook na webe **a** poštovú schránku sa nepodarilo nájsť z dôvodu chyby, konto, ktoré ste použili na pripojenie k Outlooku na webe, nemá licenciu na Exchange Online, a preto ku kontu nie je priradená žiadna poštová schránka.</span><span class="sxs-lookup"><span data-stu-id="f4151-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="f4151-104">Správca môže vášmu kontu priradiť licenciu pomocou týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="f4151-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="f4151-105">Otvorte Centrum [spravovania služby Microsoft 365,](https://portal.office.com/adminportal/home#/homepage) prejdite do časti Aktívni používatelia v časti Používatelia a vyberte používateľa, ktorý chybu zobrazuje.  </span><span class="sxs-lookup"><span data-stu-id="f4151-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="f4151-106">Na stránke používateľa, ktorá sa  otvorí, prejdite do časti  Licencie a aplikácie, vyberte príslušnú hodnotu Umiestnenia a priraďte licenciu, ktorá obsahuje Exchange Online (rozbaľte licenciu a zobrazte jej podrobnosti).</span><span class="sxs-lookup"><span data-stu-id="f4151-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="f4151-107">Po dokončení kliknite na tlačidlo **Uložiť zmeny**.</span><span class="sxs-lookup"><span data-stu-id="f4151-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="f4151-108">V niektorých prípadoch, ak je licencia už priradená k používateľskému kontu, odstránenie a opätovné priradenie licencie pomáha vyriešiť problém a správne ho poskytnúť v systéme:</span><span class="sxs-lookup"><span data-stu-id="f4151-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="f4151-109">Skontrolujte, či sú vaše predplatné na M365 Exchange Online (a iné, ak máte nejaké) aktuálne a či uplynula platnosť len nedávno.</span><span class="sxs-lookup"><span data-stu-id="f4151-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="f4151-110">Keď ste sa uistili, že platnosť predplatného nelynula a ku kontu používateľa bola priradená platná licencia, môže trvať až 24 hodín, kým sa zistí platnosť licencie, takže možno budete musieť počkať, kým sa problém vyrieši.</span><span class="sxs-lookup"><span data-stu-id="f4151-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="f4151-111">Ďalšie informácie nájdete v téme [Priradenie a správa licencií.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="f4151-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>