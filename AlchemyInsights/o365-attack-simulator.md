---
title: 2681 útoku simulátor v Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713481"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="3db25-102">Simulátor útoku v Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3db25-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="3db25-103">Ste chýbajúce útoku simulátor?</span><span class="sxs-lookup"><span data-stu-id="3db25-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="3db25-104">Attack Simulator vyžaduje **office 365 pokročilé ohrozenia ochrany plán 2 (ATP Plan 2)** alebo **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="3db25-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="3db25-105">Attack Simulator **nie** je zahrnutá v balíku Office 365 pokročilé ohrozenia ochrany plán 1 (ATP Plan 1), Office 365 Enterprise E3 alebo akékoľvek Microsoft 365 aplikácie pre podnikové predplatné.</span><span class="sxs-lookup"><span data-stu-id="3db25-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="3db25-106">Konto, ktoré používate na spustenie simulovaných útokov vyžaduje globálny správca alebo povolenia správcu zabezpečenia a viacnásobné overovanie (MFA).</span><span class="sxs-lookup"><span data-stu-id="3db25-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="3db25-107">Ďalšie informácie o požiadavkách na simulátore útoku nájdete [v tejto téme](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="3db25-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="3db25-108">Dôležité veci vedieť o **hrubou silou heslo** útoku simulácie:</span><span class="sxs-lookup"><span data-stu-id="3db25-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="3db25-109">Ak cieľový účet má MFA povolené a heslo bolo uhádnuť správne, účet nebude zobrazovať ako ohrozená (druhý overovací faktor bude neúplné).</span><span class="sxs-lookup"><span data-stu-id="3db25-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="3db25-110">Súbor s heslom nemôže byť väčší ako 10 MB.</span><span class="sxs-lookup"><span data-stu-id="3db25-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="3db25-111">Použite jedno heslo na riadok a po poslednom hesle v zozname zahrňte prázdny riadok (návrat vozíka).</span><span class="sxs-lookup"><span data-stu-id="3db25-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="3db25-112">Dôležité veci vedieť o **Spear phishing** priložiť simulácie:</span><span class="sxs-lookup"><span data-stu-id="3db25-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="3db25-113">Podľa návrhu nemôžete poskytnúť vlastnú hodnotu **adresy URL prihlasovacieho servera pre neoprávnené získavanie údajov**.</span><span class="sxs-lookup"><span data-stu-id="3db25-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="3db25-114">Ak príjemca používa povoliť správu správa [Add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) hlásiť správy ako phishing, nemusí dostávať upozornenia na správu (pretože to je simulovaný útok).</span><span class="sxs-lookup"><span data-stu-id="3db25-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="3db25-115">Prehľady: po dokončení simulovaného útoku môžete kliknutím na položku **Podrobnosti o útoku** Zobraziť zostavu.</span><span class="sxs-lookup"><span data-stu-id="3db25-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="3db25-116">Podrobné pokyny a nové funkcie v útoku simulátor, pozri [útoku simulátor v Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="3db25-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
