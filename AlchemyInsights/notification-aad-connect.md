---
title: Pripájanie k upozorneniam AAD
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037237"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="5471c-102">Pripájanie k upozorneniam AAD</span><span class="sxs-lookup"><span data-stu-id="5471c-102">Notification AAD Connect</span></span>

- <span data-ttu-id="5471c-103">Uistite sa, že máte oprávnenie na vykonanie operácie.</span><span class="sxs-lookup"><span data-stu-id="5471c-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="5471c-104">Globálni správcovia majú predvolene prístup.</span><span class="sxs-lookup"><span data-stu-id="5471c-104">Global Admins have access by default.</span></span> <span data-ttu-id="5471c-105">Okrem toho môžete použiť [riadenie prístupu na základe rolí](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) na delegovanie povolenia na registráciu prispievateľovi.</span><span class="sxs-lookup"><span data-stu-id="5471c-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="5471c-106">Uistite sa, že sú povolené požadované koncové body a nie je blokovaný v dôsledku brány firewall.</span><span class="sxs-lookup"><span data-stu-id="5471c-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="5471c-107">Podrobnosti nájdete v téme [požiadavky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="5471c-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="5471c-108">Registrácia môže zlyhať z dôvodu odchádzajúcej komunikácie, ktorá je podrobená kontrole SSL prostredníctvom sieťovej vrstvy.</span><span class="sxs-lookup"><span data-stu-id="5471c-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="5471c-109">Skontrolujte, či ste overili nastavenie oznámení pre službu Azure AD Connect Health a skontrolujte nastavenie.</span><span class="sxs-lookup"><span data-stu-id="5471c-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="5471c-110">Ak chcete zistiť, ako nakonfigurovať nastavenia oznámení pre oznámenia o stave pripojenia služby Azure AD, pozrite si túto [príručku](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="5471c-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="5471c-111">Ak chcete získať ďalšie informácie o zostave synchronizácie so službou AAD Connect Health a o tom, ako si ju stiahnuť, pozrite si tému [synchronizácia na úrovni objektov](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="5471c-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="5471c-112">Riešenie problémov s aplikáciou AAD Connect Health nájdete [v príručke na riešenie problémov s funkciou AAD pripojenie upozornení o stave údajov o zdraví](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) a v prípade najčastejšie kladených otázok sa nachádzajú v téme [bežné problémy pri inštalácii](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="5471c-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
