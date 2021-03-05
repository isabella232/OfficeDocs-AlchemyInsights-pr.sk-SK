---
title: Problém s funkciou AAD Connect Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483119"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="99254-102">Problém s funkciou AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="99254-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="99254-103">Uistite sa, že máte oprávnenie na vykonanie operácie.</span><span class="sxs-lookup"><span data-stu-id="99254-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="99254-104">Globálni správcovia majú predvolene prístup.</span><span class="sxs-lookup"><span data-stu-id="99254-104">Global Admins have access by default.</span></span> <span data-ttu-id="99254-105">Okrem toho môžete použiť [riadenie prístupu na základe rolí](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) na delegovanie povolenia na registráciu prispievateľovi.</span><span class="sxs-lookup"><span data-stu-id="99254-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="99254-106">Uistite sa, že sú povolené požadované koncové body a nie je blokovaný v dôsledku brány firewall.</span><span class="sxs-lookup"><span data-stu-id="99254-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="99254-107">Podrobnosti nájdete v téme [požiadavky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="99254-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="99254-108">Registrácia môže zlyhať z dôvodu odchádzajúcej komunikácie, ktorá je podrobená kontrole SSL prostredníctvom sieťovej vrstvy.</span><span class="sxs-lookup"><span data-stu-id="99254-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="99254-109">Skontrolujte, či ste overili nastavenie oznámení v službe Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="99254-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="99254-110">Skontrolujte nastavenie.</span><span class="sxs-lookup"><span data-stu-id="99254-110">Please review your setting.</span></span> <span data-ttu-id="99254-111">Táto [príručka](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vám pomôže pochopiť, ako nakonfigurovať nastavenia oznámení pre oznámenia o stave pripojenia služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="99254-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="99254-112">Ak chcete získať ďalšie informácie o zostave synchronizácie so službou AAD Connect Health a o tom, ako si ju stiahnuť, pozrite si tému [synchronizácia na úrovni objektov](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="99254-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="99254-113">Ak chcete riešiť problémy so zobrazovaním upozornení o stave pripojenia AAD, postupujte podľa pokynov na [Riešenie problémov s funkciou AAD pripojenie upozornení o stave údajov o zdraví](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) a v prípade najčastejšie kladených otázok nájdete v téme [bežné problémy so stavom inštalácie](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="99254-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
