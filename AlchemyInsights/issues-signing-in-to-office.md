---
title: Problémy s prihlásením do aplikácií Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695302"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="393fb-102">Prázdna prihlasovacia obrazovka v aplikáciách Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="393fb-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="393fb-103">Ak chcete tento problém vyriešiť, vyskúšajte tento postup:</span><span class="sxs-lookup"><span data-stu-id="393fb-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="393fb-104">Nainštalujte si najnovšie aktualizácie pre [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="393fb-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="393fb-105">Obnovenie možností programu Internet Explorer: prechod na položku **Nástroje**  >  **internetu**–  >  **Rozšírené**  >  **Obnovenie nastavení programu Internet Explorer** (Všimnite si, že stratíte vlastné nastavenia) a potom sa znova skúste prihlásiť do balíka Office.</span><span class="sxs-lookup"><span data-stu-id="393fb-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="393fb-106">Vypnite funkciu Windows Defender Application Guard (WDAG) alebo podobnú bránu firewall alebo program na ochranu pred vírusmi:</span><span class="sxs-lookup"><span data-stu-id="393fb-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="393fb-107">V ovládacom paneli prejdite na položku **programy**a potom vyberte položku **Zapnúť alebo vypnúť súčasti systému Windows**.</span><span class="sxs-lookup"><span data-stu-id="393fb-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="393fb-108">Ak je zapnutá ochrana aplikácií Windows Defender, skúste ju vypnúť.</span><span class="sxs-lookup"><span data-stu-id="393fb-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="393fb-109">**Poznámka:** Možno bude potrebné reštartovať počítač.</span><span class="sxs-lookup"><span data-stu-id="393fb-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="393fb-110">Uistite sa, že doplnok Microsoft. AAD. BrokerPlugin [AAD](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie je blokovaný žiadnou aplikáciou alebo bránou firewall alebo programom na ochranu pred vírusmi.</span><span class="sxs-lookup"><span data-stu-id="393fb-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="393fb-111">[Vymazanie poverení balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.</span><span class="sxs-lookup"><span data-stu-id="393fb-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="393fb-112">**Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na 16,0.</span><span class="sxs-lookup"><span data-stu-id="393fb-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="393fb-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="393fb-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="393fb-114">Ďalšie informácie nájdete v téme [problémy s pripojením pri prihlasovaní po aktualizácii na Office 2016 build 16.0.7967 vo Windowse 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="393fb-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>