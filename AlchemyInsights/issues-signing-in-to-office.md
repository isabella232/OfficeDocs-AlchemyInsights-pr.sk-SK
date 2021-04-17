---
title: Problémy pri prihlasovaní do aplikácií Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833054"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="65c9d-102">Prázdna prihlasovacia obrazovka v aplikáciách Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="65c9d-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="65c9d-103">Ak chcete tento problém vyriešiť, vyskúšajte tento postup:</span><span class="sxs-lookup"><span data-stu-id="65c9d-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="65c9d-104">Nainštalujte najnovšie aktualizácie pre [Windows a](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="65c9d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="65c9d-105">Obnovenie možností programu Internet Explorer: Prejdite na položku Nástroje – možnosti siete Internet – rozšírené obnovenie výrobných nastavení  >    >    >  **programu Internet Explorer** (upozorňujeme, že stratíte vlastné nastavenia) a potom sa znova prihláste do balíka Office.</span><span class="sxs-lookup"><span data-stu-id="65c9d-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="65c9d-106">Zakážte Windows Defender Application Guard (WDAG) alebo podobný firewall či antivírusový program:</span><span class="sxs-lookup"><span data-stu-id="65c9d-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="65c9d-107">V ovládacom paneli prejdite na **položku Programy** a potom vyberte položku Zapnúť alebo vypnúť funkcie **systému Windows.**</span><span class="sxs-lookup"><span data-stu-id="65c9d-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="65c9d-108">Ak je funkcia Windows Defender Application Guard zapnutá, skúste ju vypnúť.</span><span class="sxs-lookup"><span data-stu-id="65c9d-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="65c9d-109">**Poznámka:** Je možné, že budete musieť reštartovať počítač.</span><span class="sxs-lookup"><span data-stu-id="65c9d-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="65c9d-110">Skontrolujte, či doplnok Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie je blokovaný aplikáciou, bránou firewall/antivírusovým programom.</span><span class="sxs-lookup"><span data-stu-id="65c9d-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="65c9d-111">[Odstráňte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.</span><span class="sxs-lookup"><span data-stu-id="65c9d-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="65c9d-112">**Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na hodnotu 16.0.</span><span class="sxs-lookup"><span data-stu-id="65c9d-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="65c9d-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="65c9d-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="65c9d-114">Ďalšie informácie nájdete v téme Problémy s pripojením pri prihlasovaní po aktualizácii na [zostavu 16.0.7967 balíka Office 2016 vo Windowse 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="65c9d-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>