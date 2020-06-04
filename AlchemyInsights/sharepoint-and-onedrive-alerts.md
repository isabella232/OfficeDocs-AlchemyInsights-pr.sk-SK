---
title: Oneskorenia pri prijímaní upozornení na SharePoint a OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563525"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="310b5-102">Oneskorenia pri prijímaní upozornení na SharePoint a OneDrive</span><span class="sxs-lookup"><span data-stu-id="310b5-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="310b5-103">Najprv skontrolujte priečinok Nevyžiadaná pošta alebo Spam v e-maile.</span><span class="sxs-lookup"><span data-stu-id="310b5-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="310b5-104">Ak **sú všetky upozornenia z viacerých súborov alebo knižníc oneskorené,** navštívte [tabuľu Stav služby](https://portal.office.com/adminportal/home?ref=/servicehealth) a skontrolujte, či sa nenachádzajú všetky upozornenia alebo incidenty, ktoré sa môžu vyskytnúť v službe SharePoint alebo Exchange.</span><span class="sxs-lookup"><span data-stu-id="310b5-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="310b5-105">Problém môže byť s možnosťou výstrahy SharePoint alebo oneskorenia e-mailov prostredníctvom servera Exchange.</span><span class="sxs-lookup"><span data-stu-id="310b5-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="310b5-106">Všimnite si tiež, či sa doručuje iný e-mail – ak nie, problém je pravdepodobne s oneskorením servera Exchange.</span><span class="sxs-lookup"><span data-stu-id="310b5-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="310b5-107">Ak **sa nedoručuje individuálne upozornenie z konkrétneho súboru alebo knižnice**, pokúste sa ho odstrániť a znova vytvoriť.</span><span class="sxs-lookup"><span data-stu-id="310b5-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="310b5-108">Ak chcete znova vytvoriť upozornenie, pozrite si tému [Správa, zobrazenie alebo odstránenie upozornení SharePointu.](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)</span><span class="sxs-lookup"><span data-stu-id="310b5-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="310b5-109">Upozornenia nie je možné odoslať distribučnej skupine.</span><span class="sxs-lookup"><span data-stu-id="310b5-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="310b5-110">Podporované sú iba skupiny Zabezpečenie a O365.</span><span class="sxs-lookup"><span data-stu-id="310b5-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="310b5-111">Šablóny e-mailov s upozornením nie je možné prispôsobiť.</span><span class="sxs-lookup"><span data-stu-id="310b5-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="310b5-112">Na dosiahnutie týchto cieľov musíte použiť pracovný postup služby Microsoft Flow alebo SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="310b5-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
