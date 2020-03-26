---
title: Migrácia do SharePointu Online prostredníctvom správcu migrácie
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932371"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="9b454-102">Migrácia do SharePointu Online prostredníctvom správcu migrácie</span><span class="sxs-lookup"><span data-stu-id="9b454-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="9b454-103">**Dôležité**: Mnoho zákazníkov SharePointu Online a OneDrivu spúšťa dôležité podnikové aplikácie s pomocou služby, ktorá beží na pozadí.</span><span class="sxs-lookup"><span data-stu-id="9b454-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9b454-104">Patrí sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="9b454-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9b454-105">V tomto neobvyklom období podnikáme kroky, aby boli služby SharePoint Online a OneDrive i naďalej vysoko dostupné a spoľahlivé pre vašich používateľov, ktorí sa v súčasnosti viac ako zvyčajne spoliehajú na túto službu pri práci na diaľku.</span><span class="sxs-lookup"><span data-stu-id="9b454-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9b454-106">Na dosiahnutie tohto cieľa sme implementovali prísnejšie obmedzenia aplikácií na pozadí (migrácia, DLP a riešenia zálohovania) počas denných hodín pracovných dní.</span><span class="sxs-lookup"><span data-stu-id="9b454-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9b454-107">Mali by ste očakávať, že tieto aplikácie dosiahnu v týchto časoch veľmi obmedzenú priepustnosť.</span><span class="sxs-lookup"><span data-stu-id="9b454-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9b454-108">Počas večerných a víkendových hodín pre príslušnú oblasť však bude služba pripravená na spracovanie významne vyššieho objemu požiadaviek z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="9b454-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9b454-109">**Správca migrácie**</span><span class="sxs-lookup"><span data-stu-id="9b454-109">**Migration Manager**</span></span>

<span data-ttu-id="9b454-110">Správca migrácie sa nachádza v modernom centre spravovania služby SharePoint a prevedie vás nastavením klientov a vytvorením vašich úloh.</span><span class="sxs-lookup"><span data-stu-id="9b454-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="9b454-111">Môžete zadať globálne nastavenia alebo nastavenia na úrovni úloh, zobraziť celkový priebeh úloh a stiahnuť súhrnné zhrnutia a zostavy na úrovni úloh.</span><span class="sxs-lookup"><span data-stu-id="9b454-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="9b454-112">Začíname so Správcom migrácie</span><span class="sxs-lookup"><span data-stu-id="9b454-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="9b454-113">Nastavenie klientov Správcu migrácie</span><span class="sxs-lookup"><span data-stu-id="9b454-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="9b454-114">Nastavenia Správcu migrácie</span><span class="sxs-lookup"><span data-stu-id="9b454-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
