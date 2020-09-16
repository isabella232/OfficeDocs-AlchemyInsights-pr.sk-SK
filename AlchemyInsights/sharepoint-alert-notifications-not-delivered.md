---
title: Upozornenia na upozornenia SharePointu sa nedoručujú
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751258"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="2d6c8-102">Upozornenia na upozornenia SharePointu sa nedoručujú</span><span class="sxs-lookup"><span data-stu-id="2d6c8-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="2d6c8-103">Skontrolujte priečinok nevyžiadanej pošty v e-maile, pretože niekedy sa môžu vyskytnúť upozornenia.</span><span class="sxs-lookup"><span data-stu-id="2d6c8-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="2d6c8-104">Zistite, či sa nezobrazia **všetky upozornenia** alebo ak sa nedoručuje **individuálne upozornenie** zo špecifického súboru alebo knižnice.</span><span class="sxs-lookup"><span data-stu-id="2d6c8-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="2d6c8-105">**Jednotlivé upozornenia sa nedoručujú**: Ak sa nedoručuje individuálne upozornenie zo špecifického súboru alebo knižnice, môžete sa pokúsiť o jeho odstránenie a opätovné vytvorenie.</span><span class="sxs-lookup"><span data-stu-id="2d6c8-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="2d6c8-106">Ďalšie informácie o opätovnom vytvorení upozornenia nájdete v téme [Správa, zobrazenie alebo odstránenie upozornení SharePointu](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="2d6c8-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="2d6c8-107">**Všetky upozornenia sa nedoručujú**: Ak sa nedoručujú všetky upozornenia z viacerých súborov alebo knižníc, prejdite na [tabuľu stavu služby](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) a vyhľadajte všetky upozornenia alebo incidenty, ktoré sa môžu vyskytnúť v SharePointe alebo Exchangei.</span><span class="sxs-lookup"><span data-stu-id="2d6c8-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="2d6c8-108">Problém môže byť s funkciou upozornenia SharePointu alebo oneskorením v e-mailoch prostredníctvom servera Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d6c8-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="2d6c8-109">Bude tiež dôležité upozorniť na to, či sa doručujú iné e-maily, a ak nie, problém je pravdepodobne s oneskorením pri výmene.</span><span class="sxs-lookup"><span data-stu-id="2d6c8-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="2d6c8-110">Najčastejšie otázky o upozorneniach:</span><span class="sxs-lookup"><span data-stu-id="2d6c8-110">FAQ on alerts:</span></span>

- <span data-ttu-id="2d6c8-111">Nie je možné odosielať upozornenia do distribučnej skupiny, podporované sú len skupiny zabezpečenia a služby O365.</span><span class="sxs-lookup"><span data-stu-id="2d6c8-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="2d6c8-112">Nie je možné prispôsobiť šablóny upozornení e-mailov, na dosiahnutie týchto úloh je potrebné použiť pracovný postup Microsoft FLOW alebo SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="2d6c8-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="2d6c8-113">Súvisiace témy</span><span class="sxs-lookup"><span data-stu-id="2d6c8-113">Related Topics</span></span>

<span data-ttu-id="2d6c8-114">Chcete vyskúšať Microsoft flow v SharePointe Online?</span><span class="sxs-lookup"><span data-stu-id="2d6c8-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="2d6c8-115">Vytvorenie toku</span><span class="sxs-lookup"><span data-stu-id="2d6c8-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="2d6c8-116">SharePoint a tok</span><span class="sxs-lookup"><span data-stu-id="2d6c8-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
