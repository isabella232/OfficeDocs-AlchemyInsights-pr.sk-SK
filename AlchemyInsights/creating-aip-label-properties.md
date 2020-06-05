---
title: Vytvorenie politiky označenia AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569511"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="824ca-102">Vytvorenie politiky označenia AIP</span><span class="sxs-lookup"><span data-stu-id="824ca-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="824ca-103">Štítky Azure Information Protection(AIP) možno použiť s celým radom údajov, ktoré organizácia zvyčajne vytvára a ukladá, od najnižšej klasifikácie osobných údajov, až po najvyššiu klasifikáciu vysoko dôverných údajov.</span><span class="sxs-lookup"><span data-stu-id="824ca-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="824ca-104">Azure politiky ochrany informácií sa vzťahujú na Azure Information Protection (AIP) klasickéklienta a nie [AIP Unified označenie klienta](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="824ca-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="824ca-105">V politike AIP môžete nakonfigurovať viacero prvkov vrátane možností, ako napríklad:</span><span class="sxs-lookup"><span data-stu-id="824ca-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="824ca-106">Možnosť, pre ktorú štítok umožní správcom alebo používateľom klasifikovať a ochranu (voliteľné) dokumenty a e-maily</span><span class="sxs-lookup"><span data-stu-id="824ca-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="824ca-107">Možnosť vynútiť klasifikáciu pri ukladaní dokumentov a odosielaní e-mailov používateľmi</span><span class="sxs-lookup"><span data-stu-id="824ca-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="824ca-108">Možnosť automatického označovania e-mailovej správy na základe jej príloh.</span><span class="sxs-lookup"><span data-stu-id="824ca-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="824ca-109">Možnosť kontroly, či sa v aplikáciách balíka Office zobrazuje panel na ochranu informácií</span><span class="sxs-lookup"><span data-stu-id="824ca-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="824ca-110">Ďalšie možnosti a informácie o politikách azure ochranu informácií nájdete v téme: [Prehľad politiky ochrany informácií platformy Azure.](https://docs.microsoft.com/azure/information-protection/overview-policy)</span><span class="sxs-lookup"><span data-stu-id="824ca-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="824ca-111">Ďalšie užitočné zdroje týkajúce sa politík AIP nájdete v témach:</span><span class="sxs-lookup"><span data-stu-id="824ca-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="824ca-112">Kurz: Konfigurácia nastavenia politiky ochrany informácií azure a vytvorenie nového štítka</span><span class="sxs-lookup"><span data-stu-id="824ca-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="824ca-113">Konfigurácia politiky Azure ochranu informácií</span><span class="sxs-lookup"><span data-stu-id="824ca-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="824ca-114">Vytvorenie a konfigurácia menoviek citlivosti a ich politík</span><span class="sxs-lookup"><span data-stu-id="824ca-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="824ca-115">Príručky pre bežné scenáre, ktoré používajú službu Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="824ca-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="824ca-116">Preskúmanie dokumentácie azure information protection</span><span class="sxs-lookup"><span data-stu-id="824ca-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="824ca-117">Požiadavky na ochranu informácií azure</span><span class="sxs-lookup"><span data-stu-id="824ca-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="824ca-118">Kurz rýchleho spustenia pre službu Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="824ca-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="824ca-119">Stiahnuť Azure informácie ochrany klienta</span><span class="sxs-lookup"><span data-stu-id="824ca-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)