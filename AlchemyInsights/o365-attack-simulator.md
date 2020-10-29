---
title: Simulátor útoku 2681 v Microsoft 365
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801566"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="fd036-102">Simulátor útoku v programe Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="fd036-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="fd036-103">Chýba vám simulátor útoku?</span><span class="sxs-lookup"><span data-stu-id="fd036-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="fd036-104">Simulátor útoku vyžaduje **program Microsoft Defender pre office 365 Plan 2 (ATP Plan 2)** alebo **Office 365 Enterprise E5** .</span><span class="sxs-lookup"><span data-stu-id="fd036-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="fd036-105">Simulátor útoku **nie** je zahrnutý v programe Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3 ani v ktorejkoľvek aplikácii Microsoft 365 for Business.</span><span class="sxs-lookup"><span data-stu-id="fd036-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="fd036-106">Konto, ktoré používate na spustenie simulovaných útokov, vyžaduje globálny správca alebo povolenia správcu zabezpečenia a viacnásobné overovanie (MFA).</span><span class="sxs-lookup"><span data-stu-id="fd036-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="fd036-107">Ďalšie informácie o požiadavkách útoku simulátora nájdete v [tejto téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="fd036-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="fd036-108">Dôležité informácie o simuláciách útoku **brutálnych síl na heslo** :</span><span class="sxs-lookup"><span data-stu-id="fd036-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="fd036-109">Ak má cieľové konto zapnuté MFA a heslo sa nesprávne zobrazilo, konto sa nebude zobrazovať ako ohrozené (druhý overovací faktor bude neúplný).</span><span class="sxs-lookup"><span data-stu-id="fd036-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="fd036-110">Súbor s heslom nemôže byť väčší ako 10 MB.</span><span class="sxs-lookup"><span data-stu-id="fd036-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="fd036-111">Použite jedno heslo na jeden riadka a do zoznamu pridajte prázdny (znak konca riadka).</span><span class="sxs-lookup"><span data-stu-id="fd036-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="fd036-112">Dôležité informácie o tom, ako **neoprávnené získavanie údajov** o službe kopije:</span><span class="sxs-lookup"><span data-stu-id="fd036-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="fd036-113">Návrhom nie je možné poskytnúť vlastnú hodnotu pre **URL adresu prihlasovacieho servera pre neoprávnené získavanie údajov** .</span><span class="sxs-lookup"><span data-stu-id="fd036-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="fd036-114">Ak príjemca použije [doplnok povoliť správu zostavy](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) na nahlásenie správy ako neoprávneného získavania údajov, možno nebudete dostávať upozornenia na správu (pretože ide o simulovaný útok).</span><span class="sxs-lookup"><span data-stu-id="fd036-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="fd036-115">Zostavy: po dokončení simulovaného útoku môžete kliknutím na položku Podrobnosti o **útoku** Zobraziť zostavu.</span><span class="sxs-lookup"><span data-stu-id="fd036-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="fd036-116">Podrobné pokyny a nové funkcie v simulátore útoku nájdete [v téme simulátor útoku v Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="fd036-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
