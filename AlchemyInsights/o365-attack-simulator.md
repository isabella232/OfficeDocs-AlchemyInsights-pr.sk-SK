---
title: 2681 Attack Simulator v Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545741"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="d0eae-102">Attack Simulator in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d0eae-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="d0eae-103">Chýba vám Attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="d0eae-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="d0eae-104">Attack Simulator vyžaduje **microsoft Defender pre Office 365 Plan 2** alebo Office 365 Enterprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="d0eae-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="d0eae-105">Attack Simulator nie **je** súčasťou programu Microsoft Defender pre Office 365 Plan 1, Office 365 Enterprise E3 ani žiadne Aplikácie Microsoft 365 pre podnikateľov predplatné.</span><span class="sxs-lookup"><span data-stu-id="d0eae-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="d0eae-106">Konto, ktoré používate na spustenie simulovaných útokov, vyžaduje povolenia globálneho správcu alebo správcu zabezpečenia a viacfaktorové overovanie (MFA).</span><span class="sxs-lookup"><span data-stu-id="d0eae-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="d0eae-107">Ďalšie informácie o požiadavkách na Attack Simulator nájdete v [tejto téme.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="d0eae-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="d0eae-108">Dôležité informácie o **simuláciách útokov Brute Force Password:**</span><span class="sxs-lookup"><span data-stu-id="d0eae-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="d0eae-109">Ak má cieľové konto zapnuté viacfaktorové overovanie a heslo bolo správne uhádnuť, konto sa nebude zobrazovať ako zneužiné (druhý overovací faktor bude neúplný).</span><span class="sxs-lookup"><span data-stu-id="d0eae-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="d0eae-110">Súbor hesiel nemôže byť väčší ako 10 MB.</span><span class="sxs-lookup"><span data-stu-id="d0eae-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="d0eae-111">Použite jedno heslo na jeden riadok a za posledné heslo v zozname uveďte prázdny riadok (koniec riadka).</span><span class="sxs-lookup"><span data-stu-id="d0eae-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="d0eae-112">Dôležité veci, ktoré by ste mali vedieť o **tom, že Phishing prikladá** simulácie:</span><span class="sxs-lookup"><span data-stu-id="d0eae-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="d0eae-113">Nie je možné poskytnúť vlastnú hodnotu prihlasovacej adresy servera neoprávneného získavania **údajov na základe návrhu.**</span><span class="sxs-lookup"><span data-stu-id="d0eae-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="d0eae-114">Ak príjemca použije [](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) doplnok Povoliť správu správy na nahlásenie správy ako neoprávneného získavania údajov, je možné, že sa na správu nebudú prijímať upozornenia (pretože ide o simulovaný útok).</span><span class="sxs-lookup"><span data-stu-id="d0eae-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="d0eae-115">Zostavy: Po dokončení simulovaného útoku môžete kliknutím na položku **Podrobnosti o útoke** zobraziť zostavu.</span><span class="sxs-lookup"><span data-stu-id="d0eae-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="d0eae-116">Podrobné pokyny a nové funkcie v attack Simulatore nájdete v téme [Attack Simulator v Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="d0eae-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
