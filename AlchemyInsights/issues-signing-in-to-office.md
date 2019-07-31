---
title: Problémy s prihlásením do aplikácie balíka Office
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938335"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="03728-102">Prázdne prihlasovacej obrazovky v aplikáciách balíka Office</span><span class="sxs-lookup"><span data-stu-id="03728-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="03728-103">Ak chcete vyriešiť tento problém, skúste nasledovné:</span><span class="sxs-lookup"><span data-stu-id="03728-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="03728-104">Nainštalujte najnovšie aktualizácie pre [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="03728-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="03728-105">Vynulovanie nastavení programu Internet Explorer: Prejdite na **Nástroje** > **Možnosti siete Internet** > **Rozšírené** > **Internet Explorer – obnovenie pôvodného nastavenia** (Všimnite si, že stratíte vlastné nastavenia) a potom sa pokúste znova prihlásiť do kancelárie.</span><span class="sxs-lookup"><span data-stu-id="03728-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="03728-106">Zakázať Windows Defender aplikácie stráž (WDAG) alebo akýkoľvek podobný firewall alebo anti-virus program:</span><span class="sxs-lookup"><span data-stu-id="03728-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="03728-107">V ovládacom paneli, prejdite na položku **programy**a potom vyberte **alebo vypnúť súčasti systému Windows**.</span><span class="sxs-lookup"><span data-stu-id="03728-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="03728-108">Ak je zapnutý Windows Defender aplikačného ochrancu, skúste ju vypnúť.</span><span class="sxs-lookup"><span data-stu-id="03728-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="03728-109">**Poznámka:** Budete musieť reštartovať počítač.</span><span class="sxs-lookup"><span data-stu-id="03728-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="03728-110">Uistite sa, že Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) je neblokuje žiadne aplikácie alebo firewall/anti-anti-virus program.</span><span class="sxs-lookup"><span data-stu-id="03728-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="03728-111">[Jasné úradu poverení](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou poverení správcu systému Windows.</span><span class="sxs-lookup"><span data-stu-id="03728-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="03728-112">**Poznámka:** Cesty databázy registry Office 2016 zmenili 16,0.</span><span class="sxs-lookup"><span data-stu-id="03728-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="03728-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="03728-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="03728-114">Ďalšie informácie nájdete v téme [pripojenie problémy v sign-in po aktualizácii Office 2016 build 16.0.7967 v systéme Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="03728-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>