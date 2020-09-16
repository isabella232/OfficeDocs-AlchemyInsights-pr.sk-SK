---
title: Odložiť inováciu tímu
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
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741786"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="858e1-102">Ako odložiť inováciu na teams riadený spoločnosťou Microsoft</span><span class="sxs-lookup"><span data-stu-id="858e1-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="858e1-103">**Dôležité**: Tento problém vám môžeme pomôcť pri používaní diagnostických podpory, ale vyzerá to, že nepoužívate nové centrum spravovania.</span><span class="sxs-lookup"><span data-stu-id="858e1-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="858e1-104">Ak chcete použiť nové centrum spravovania, posuňte prepínač v pravom hornom rohu, v ktorom sa nachádza **nové centrum spravovania** napravo.</span><span class="sxs-lookup"><span data-stu-id="858e1-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="858e1-105">Pomocou nového centra spravovania kliknite na položku **potrebujete pomoc?** widget, zadajte slovné spojenie "odložiť inováciu na teams" a potom postupujte podľa pokynov na spustenie diagnostiky.</span><span class="sxs-lookup"><span data-stu-id="858e1-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="858e1-106">Ak ste dostali oznámenie o automatickej inovácii od spoločnosti Microsoft z Skypu for Business do aplikácie Microsoft teams a chcete odložiť automatizovanú inováciu na neskorší dátum, globálny správca sa môže prihlásiť na [portáli teams admin](https://admin.teams.microsoft.com/dashboard) a po výbere tlačidla **stavu obnovenia** v časti Inovácia v programe Microsoft teams vyberte tlačidlo **odložiť** .</span><span class="sxs-lookup"><span data-stu-id="858e1-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="858e1-107">Ak chcete zobraziť nový dátum automatickej inovácie nájomníka na Microsoft Teams, obnovte stránku portálu na správu tímov.</span><span class="sxs-lookup"><span data-stu-id="858e1-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="858e1-108">**Poznámka:** Tlačidlo **odložiť** bude k dispozícii len v prípade, že ste dostali oznámenie centra správ o automatickej inovácii.</span><span class="sxs-lookup"><span data-stu-id="858e1-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="858e1-109">Globálni správcovia môžu tiež spustiť [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) , kde získate ďalšie informácie o aktuálnom stave inovácie.</span><span class="sxs-lookup"><span data-stu-id="858e1-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
