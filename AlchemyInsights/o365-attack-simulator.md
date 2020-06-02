---
title: 2681 Útok Simulátor v Microsoft 365
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
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506753"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="30c1d-102">Útok Simulátor v Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="30c1d-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="30c1d-103">Chýba vám Simulátor útoku?</span><span class="sxs-lookup"><span data-stu-id="30c1d-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="30c1d-104">Simulátor útoku vyžaduje **rozšírený plán ochrany pred hrozbami služieb Office 365 2 (plán ATP 2)** alebo **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="30c1d-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="30c1d-105">Simulátor Útok **nie** je súčasťou rozšíreného plánu ochrany pred hrozbami služieb Office 365 1 (plán ATP 1), office 365 Enterprise E3 ani v žiadnom prípade v aplikáciách Microsoft 365 pre podnikové predplatné.</span><span class="sxs-lookup"><span data-stu-id="30c1d-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="30c1d-106">Konto, ktoré používate na spustenie simulovaných útokov, vyžaduje povolenia globálneho správcu alebo správcu zabezpečenia a viacnásobné overovanie (MFA).</span><span class="sxs-lookup"><span data-stu-id="30c1d-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="30c1d-107">Ďalšie informácie o požiadavkách attack simulator nájdete [v tejto téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="30c1d-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="30c1d-108">Dôležité veci vedieť o **Simulácia útoku Brute Force Password:**</span><span class="sxs-lookup"><span data-stu-id="30c1d-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="30c1d-109">Ak cieľový účet má MFA povolené a heslo uhádol správne, konto sa nezobrazí ako ohrozená (druhý overovací faktor bude neúplný).</span><span class="sxs-lookup"><span data-stu-id="30c1d-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="30c1d-110">Súbor s heslom nemôže byť väčší ako 10 MB.</span><span class="sxs-lookup"><span data-stu-id="30c1d-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="30c1d-111">Použite jedno heslo na riadok a za posledné heslo v zozname zadajte prázdny riadok (návrat riadka).</span><span class="sxs-lookup"><span data-stu-id="30c1d-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="30c1d-112">Dôležité informácie o **Spear Phishing** pripojiť simulácie:</span><span class="sxs-lookup"><span data-stu-id="30c1d-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="30c1d-113">Zámerne nie je možné zadať vlastnú hodnotu pre **adresu URL prihlasovacieho servera neoprávneného získavania údajov**.</span><span class="sxs-lookup"><span data-stu-id="30c1d-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="30c1d-114">Ak príjemca používa doplnok [Povoliť správu na](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) hlásenie správy ako neoprávnené získavanie údajov, pravdepodobne nebudete dostávať upozornenia na správu (pretože ide o simulovaný útok).</span><span class="sxs-lookup"><span data-stu-id="30c1d-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="30c1d-115">Správy: Po dokončení simulovaného útoku môžete kliknúť na položku **Podrobnosti o útoku** a zobraziť prehľad.</span><span class="sxs-lookup"><span data-stu-id="30c1d-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="30c1d-116">Podrobné pokyny a nové funkcie v aplikácii Attack Simulator nájdete v téme [Simulátor útoku v aplikácii Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="30c1d-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
