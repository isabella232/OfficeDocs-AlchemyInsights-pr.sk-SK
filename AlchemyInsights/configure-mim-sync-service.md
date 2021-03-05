---
title: Konfigurácia služby synchronizácie MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482898"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="0bcf0-102">Konfigurácia služby synchronizácie MIM</span><span class="sxs-lookup"><span data-stu-id="0bcf0-102">Configure MIM Sync service</span></span>

<span data-ttu-id="0bcf0-103">Služba synchronizácie Microsoft Identity Manager (MIM) je súčasťou MIM.</span><span class="sxs-lookup"><span data-stu-id="0bcf0-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="0bcf0-104">Ide o centralizovanú lokálnu službu, ktorá ukladá a integruje informácie o organizáciách s viacerými lokálnymi adresármi a databázami.</span><span class="sxs-lookup"><span data-stu-id="0bcf0-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="0bcf0-105">Problém s synchronizáciou MIM môžete vyriešiť v prípade, že problém bol vyriešený v poslednej aktualizácii na MIM alebo je jedným z ďalších problémov uvedených v časti nižšie.</span><span class="sxs-lookup"><span data-stu-id="0bcf0-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="0bcf0-106">**Odporúčané kroky**</span><span class="sxs-lookup"><span data-stu-id="0bcf0-106">**Recommended steps**</span></span>

1. <span data-ttu-id="0bcf0-107">Uistite sa, že používate nedávnu aktualizáciu synchronizácie MIM a skontrolujte poznámky k [vydaniu synchronizácie Mim](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) a zistite, či sa problém vyriešil v aktualizácii.</span><span class="sxs-lookup"><span data-stu-id="0bcf0-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="0bcf0-108">Ak sa vyskytol problém s doplnkom generických protokolov LDAP, Generic SQL, Lotus Domino alebo Web Services, skontrolujte, či používate nedávnu aktualizáciu [všeobecných spojníc](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="0bcf0-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="0bcf0-109">Ak sa synchronizácia MIM spustí s chybou, prečítajte si tabuľku [chybových kódov spustiť](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) , aby ste určili možné príčiny.</span><span class="sxs-lookup"><span data-stu-id="0bcf0-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="0bcf0-110">Ak sa spustiť zastaví s **rozšírením – DLL – výnimka**, kliknite na tieto slová a otvorte okno **Vlastnosti objektu spojnice** a kliknite na položku **sledovanie zásobníka..** . a zobrazia sa ďalšie informácie o príčine, ako je to popísané v téme [rozšírenie – dll – výnimka](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="0bcf0-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="0bcf0-111">Ak sa pri synchronizácii hesla v denníku udalostí počas synchronizácie hesiel **zobrazí chybové** hlásenie o tom, že v príručke na riešenie problémov s [vyhlásením služby PCNS sa 6025 zobrazí](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)chyba 6025.</span><span class="sxs-lookup"><span data-stu-id="0bcf0-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="0bcf0-112">Ak je úplná synchronizácia s agentom správy služby FIM pomalá, skontrolujte nastavenie **automatického rastu** pre tempdb, ako je popísané v časti [Riešenie problémov s pomalým alebo zavesením úplnej synchronizácie](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="0bcf0-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="0bcf0-113">Ak sa vyskytne chyba zastaveného servera s neúspešným vytvorením-cez-Web-Services pomocou agenta správy služby FIM, prečítajte si tému [Technická podpora – informácie: zlyhanie – vytvorenie – cez – web – služby](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) na prehľad príčin.</span><span class="sxs-lookup"><span data-stu-id="0bcf0-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

