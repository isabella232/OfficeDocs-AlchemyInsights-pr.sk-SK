---
title: Oneskorenie pri prijímaní upozornení SharePointu a OneDrivu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727258"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="09a5b-102">Oneskorenie pri prijímaní upozornení SharePointu a OneDrivu</span><span class="sxs-lookup"><span data-stu-id="09a5b-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="09a5b-103">Najskôr skontrolujte priečinok nevyžiadanej pošty alebo Nevyžiadaná pošta v e-maile.</span><span class="sxs-lookup"><span data-stu-id="09a5b-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="09a5b-104">Ak **sú všetky upozornenia z viacerých súborov alebo knižníc oneskorené**, navštívte [tabuľu stavu služby](https://portal.office.com/adminportal/home?ref=/servicehealth) a skontrolujte, či sú k dispozícii upozornenia alebo incidenty, ktoré sa môžu vyskytnúť v SharePointe alebo Exchangei.</span><span class="sxs-lookup"><span data-stu-id="09a5b-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="09a5b-105">Problém môže byť s funkciou upozornenia SharePointu alebo oneskorením v e-mailoch cez Exchange.</span><span class="sxs-lookup"><span data-stu-id="09a5b-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="09a5b-106">Všimnite si tiež, či sa doručujú iné e-maily – Ak nie, problém je pravdepodobne s oneskorením pri výmene.</span><span class="sxs-lookup"><span data-stu-id="09a5b-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="09a5b-107">Ak **sa nedoručuje individuálne upozornenie zo špecifického súboru alebo knižnice**, pokúste sa ho odstrániť a znova vytvoriť.</span><span class="sxs-lookup"><span data-stu-id="09a5b-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="09a5b-108">Ďalšie informácie o opätovnom vytvorení upozornenia nájdete v téme [Správa, zobrazenie alebo odstránenie upozornení SharePointu](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="09a5b-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="09a5b-109">Upozornenia nie je možné odoslať do distribučnej skupiny.</span><span class="sxs-lookup"><span data-stu-id="09a5b-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="09a5b-110">Podporované sú len skupiny zabezpečenia a služby O365.</span><span class="sxs-lookup"><span data-stu-id="09a5b-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="09a5b-111">Nie je možné prispôsobiť šablóny upozornení e-mailom.</span><span class="sxs-lookup"><span data-stu-id="09a5b-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="09a5b-112">Na dosiahnutie týchto úloh je nutné použiť pracovný postup Microsoft Flow alebo SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="09a5b-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
