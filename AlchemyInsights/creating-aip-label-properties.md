---
title: Vytvorenie politík AIP menoviek
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732190"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="f6812-102">Vytvorenie politík AIP menoviek</span><span class="sxs-lookup"><span data-stu-id="f6812-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="f6812-103">Označenia Azure Information Protection (AIP) možno použiť s úplným rozsahom údajov, ktoré organizácia zvyčajne vytvára a ukladá, od najnižšej klasifikácie osobných údajov až po najvyššiu klasifikáciu vysoko dôverných údajov.</span><span class="sxs-lookup"><span data-stu-id="f6812-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="f6812-104">Politiky ochrany informácií Azure sa uplatňujú na klasického klienta Azure Information Protection (AIP) a nie na  [klienta AIP Unified labeling](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="f6812-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="f6812-105">Môžete nakonfigurovať viacero prvkov v politike AIP vrátane možností, ako napríklad:</span><span class="sxs-lookup"><span data-stu-id="f6812-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="f6812-106">Možnosť, pre ktorú označenie umožní správcom alebo klasifikácii a ochrane používateľov (voliteľné) dokumenty a e-maily</span><span class="sxs-lookup"><span data-stu-id="f6812-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="f6812-107">Možnosť vynútenia klasifikácie pri ukladaní dokumentov a odosielaní e-mailov používateľom</span><span class="sxs-lookup"><span data-stu-id="f6812-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="f6812-108">Možnosť automaticky označiť e-mailovú správu na základe príloh.</span><span class="sxs-lookup"><span data-stu-id="f6812-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="f6812-109">Možnosť na určenie, či sa v aplikáciách balíka Office zobrazuje panel ochrany informácií</span><span class="sxs-lookup"><span data-stu-id="f6812-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="f6812-110">Ďalšie možnosti a informácie o politikách ochrany informácií Azure nájdete v téme: [Prehľad politiky ochrany informácií Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="f6812-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="f6812-111">Ďalšie užitočné zdroje informácií o politikách AIP nájdete v témach:</span><span class="sxs-lookup"><span data-stu-id="f6812-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="f6812-112">Kurz: Konfigurácia nastavení politiky ochrany informácií Azure a vytvorenie novej menovky</span><span class="sxs-lookup"><span data-stu-id="f6812-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="f6812-113">Konfigurovanie politiky ochrany informácií Azure</span><span class="sxs-lookup"><span data-stu-id="f6812-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="f6812-114">Vytvorenie a konfigurácia označení citlivosti a ich politík</span><span class="sxs-lookup"><span data-stu-id="f6812-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="f6812-115">Príručky pre bežné scenáre, ktoré používajú ochranu informácií Azure</span><span class="sxs-lookup"><span data-stu-id="f6812-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="f6812-116">Revízia dokumentácie služby Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="f6812-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="f6812-117">Požiadavky na ochranu informácií Azure</span><span class="sxs-lookup"><span data-stu-id="f6812-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="f6812-118">Príručka so stručným návodom na ochranu informácií v službe Azure</span><span class="sxs-lookup"><span data-stu-id="f6812-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="f6812-119">Stiahnuť klienta na ochranu informácií Azure</span><span class="sxs-lookup"><span data-stu-id="f6812-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)