---
title: DLP nefunguje podľa očakávania
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932637"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="00f29-102">DLP nefunguje podľa očakávania</span><span class="sxs-lookup"><span data-stu-id="00f29-102">DLP not working as expected</span></span>

<span data-ttu-id="00f29-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="00f29-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="00f29-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="00f29-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="00f29-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="00f29-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="00f29-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="00f29-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="00f29-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="00f29-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="00f29-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="00f29-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="00f29-109">**Nastavenie DLP**</span><span class="sxs-lookup"><span data-stu-id="00f29-109">**Setting up DLP**</span></span>

<span data-ttu-id="00f29-110">Máte problémy s **únikom údajov (DLP)** v balíku Office 365 nefunguje podľa očakávania?</span><span class="sxs-lookup"><span data-stu-id="00f29-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="00f29-111">Ak áno, uistite sa, že **DLP politika** je nastavená správne, a že vaše údaje obsahuje to, čo **DLP politika** hľadá, keď sa hodnotí.</span><span class="sxs-lookup"><span data-stu-id="00f29-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="00f29-112">Politiky DLP vám umožňujú identifikovať a chrániť citlivé informácie vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="00f29-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="00f29-113">Ak chcete nastaviť politiky DLP, použite informácie [tu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="00f29-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="00f29-114">**Čo DLP politiky Hľadať**</span><span class="sxs-lookup"><span data-stu-id="00f29-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="00f29-115">Pri použití **vstavané typy citlivých informácií** v Office 365 zabezpečenia a súladu centrum, DLP politiky Hľadať špecifické vzory a prvky pri zisťovaní týchto citlivých typov.</span><span class="sxs-lookup"><span data-stu-id="00f29-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="00f29-116">**Vstavané typy citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="00f29-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="00f29-117">Informácie o vstavaných citlivých typoch a o tom, čo politika DLP vyhľadáva pri zisťovaní citlivého typu, nájdete v téme: [Aké typy citlivých informácií hľadajú](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="00f29-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="00f29-118">**Vlastné citlivé typy informácií**</span><span class="sxs-lookup"><span data-stu-id="00f29-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="00f29-119">Ak sa pokúšate vytvoriť vlastné citlivé typy informácií, použite nasledujúci článok informácie o tom, ako vytvoriť vlastný citlivý typ: [vytvoriť vlastné citlivé informácie typu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="00f29-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="00f29-120">**Testovanie politiky DLP**</span><span class="sxs-lookup"><span data-stu-id="00f29-120">**Test a DLP policy**</span></span>

<span data-ttu-id="00f29-121">Ak chcete otestovať údaje pomocou vstavaného alebo vlastného typu citlivých informácií, použite možnosť **typ testu** podľa **klasifikácie** > **citlivých typov**informácií.</span><span class="sxs-lookup"><span data-stu-id="00f29-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="00f29-122">Ďalšie informácie nájdete v téme [testovanie vlastných typov citlivých informácií](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="00f29-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="00f29-123">**Správy**</span><span class="sxs-lookup"><span data-stu-id="00f29-123">**Reports**</span></span>
  
- <span data-ttu-id="00f29-124">Získajte citlivé údaje s [prehľadom DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="00f29-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="00f29-125">Pozrite si konkrétne podrobnosti udalosti so [správou o incidente](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="00f29-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
