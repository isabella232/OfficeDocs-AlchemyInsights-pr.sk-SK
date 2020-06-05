---
title: Problémy s prihlásením do aplikácií Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579916"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="6a7c5-102">Prázdna prihlasovacia obrazovka v aplikáciách Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6a7c5-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="6a7c5-103">Ak chcete vyriešiť tento problém, vyskúšajte nasledujúci postup:</span><span class="sxs-lookup"><span data-stu-id="6a7c5-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="6a7c5-104">Nainštalujte najnovšie aktualizácie pre [systém Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="6a7c5-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="6a7c5-105">Obnovenie možností programu Internet Explorer: Prejdite na **položku Nástroje**  >  **Internet Options**  >  **Advanced**  >  **rozšíreného nastavenia programu Internet Explorer** (všimnite si, že stratíte vlastné nastavenia) a potom sa znova pokúste prihlásiť do balíka Office.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="6a7c5-106">Vypnite windows Defender Application Guard (WDAG) alebo akékoľvek podobné firewall alebo anti-virus program:</span><span class="sxs-lookup"><span data-stu-id="6a7c5-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="6a7c5-107">V ovládacom paneli prejdite do **ponuky Programs (Programy)** a potom vyberte položku **Turn Windows features on /off (Zapnúť alebo vypnúť súčasti systému Windows**).</span><span class="sxs-lookup"><span data-stu-id="6a7c5-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="6a7c5-108">Ak je zapnutá funkcia Windows Defender Application Guard, skúste ju vypnúť.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="6a7c5-109">**Upozornenie:** Možno bude potrebné reštartovať počítač.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="6a7c5-110">Uistite sa, že Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie je blokovaný žiadne aplikácie alebo firewall/anti-virus program.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="6a7c5-111">[Vymažte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou správcu poverení systému Windows.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6a7c5-112">**Upozornenie:** Cesty databázy registry pre Office 2016 sa zmenili na 16.0.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6a7c5-113">(Napr.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="6a7c5-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="6a7c5-114">Ďalšie informácie nájdete v téme [Problémy s pripojením pri prihlasovaní po aktualizácii office 2016 stavať 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="6a7c5-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>