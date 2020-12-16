---
title: Prenos služieb – presun všetkých služieb RDFE do iného predplatného
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692176"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="4b6ff-102">Prenos služieb – presun všetkých služieb RDFE do iného predplatného</span><span class="sxs-lookup"><span data-stu-id="4b6ff-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="4b6ff-103">**Premiestnenie zdrojov**</span><span class="sxs-lookup"><span data-stu-id="4b6ff-103">**Move resources**</span></span>

<span data-ttu-id="4b6ff-104">Azure zdroje je možné premiestniť do iného predplatného alebo skupiny zdrojov v rámci toho istého predplatného pomocou platformy Azure Portal, Azure PowerShell, Azure CLI alebo rozhrania REST API na presun zdrojov.</span><span class="sxs-lookup"><span data-stu-id="4b6ff-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="4b6ff-105">Skôr ako budete môcť presúvať zdroje, pozrite si tému:</span><span class="sxs-lookup"><span data-stu-id="4b6ff-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="4b6ff-106">Kontrolný zoznam pred presunom zdrojov</span><span class="sxs-lookup"><span data-stu-id="4b6ff-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="4b6ff-107">Služby, ktoré je možné premiestniť</span><span class="sxs-lookup"><span data-stu-id="4b6ff-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="4b6ff-108">Overenie premiestnenia</span><span class="sxs-lookup"><span data-stu-id="4b6ff-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="4b6ff-109">Premiestnenie poradenstva pre služby</span><span class="sxs-lookup"><span data-stu-id="4b6ff-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="4b6ff-110">Ak chcete premiestniť existujúce zdroje do inej skupiny zdrojov alebo predplatného, môžete použiť:</span><span class="sxs-lookup"><span data-stu-id="4b6ff-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="4b6ff-111">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="4b6ff-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="4b6ff-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="4b6ff-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="4b6ff-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="4b6ff-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="4b6ff-114">REST API</span><span class="sxs-lookup"><span data-stu-id="4b6ff-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="4b6ff-115">Kurz: [premiestnenie zdrojov Azure do inej skupiny zdrojov alebo predplatného](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="4b6ff-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="4b6ff-116">**Riešenie chýb v službe Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="4b6ff-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="4b6ff-117">Pozrite si články nižšie a získajte informácie o niektorých bežných chybách nasadenia Azure a prijímanie informácií na ich vyriešenie.</span><span class="sxs-lookup"><span data-stu-id="4b6ff-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="4b6ff-118">Ak nemôžete nájsť kód chyby chyby nasadenia, pozrite si tému [Vyhľadanie kódu chyby](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="4b6ff-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="4b6ff-119">Riešenie chýb nasadenia</span><span class="sxs-lookup"><span data-stu-id="4b6ff-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="4b6ff-120">Riešenie problémov so sťahovaním Azure zdrojov do novej skupiny zdrojov alebo predplatného</span><span class="sxs-lookup"><span data-stu-id="4b6ff-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="4b6ff-121">Všimnite si, že ak chcete inovovať svoje predplatné Azure, ako napríklad prechod z bezplatnej platby na Pay-as-you-go, budete musieť skonvertovať predplatné.</span><span class="sxs-lookup"><span data-stu-id="4b6ff-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="4b6ff-122">Ak chcete inovovať bezplatnú skúšobnú verziu, pozrite si tému [Inovácia bezplatnej skúšobnej verzie alebo predplatného služby Microsoft Imagine Azure na zaplatenie predplatného](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="4b6ff-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="4b6ff-123">Ak chcete zmeniť konto Pay-as-you-go, pozrite si tému [Zmena predplatného v službe Azure Pay-as-you-go do inej ponuky](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="4b6ff-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="4b6ff-124">**Pridanie alebo priradenie predplatného Azure k nájomníkovi služby Azure Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="4b6ff-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="4b6ff-125">Prihláste sa a vyberte predplatné, ktoré chcete použiť zo [stránky predplatné na portáli Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="4b6ff-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="4b6ff-126">Vyberte položku **zmeniť adresár**.</span><span class="sxs-lookup"><span data-stu-id="4b6ff-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="4b6ff-127">Skontrolujte všetky zobrazené upozornenia a potom vyberte položku **zmeniť**.</span><span class="sxs-lookup"><span data-stu-id="4b6ff-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="4b6ff-128">Adresár sa zmení na predplatné a zobrazí sa hlásenie o úspechu.</span><span class="sxs-lookup"><span data-stu-id="4b6ff-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="4b6ff-129">Pomocou prepínača *adresára* prejdite do nového adresára.</span><span class="sxs-lookup"><span data-stu-id="4b6ff-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="4b6ff-130">Ak chcete, aby sa všetko zobrazilo správne, môže trvať až 10 minút.</span><span class="sxs-lookup"><span data-stu-id="4b6ff-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="4b6ff-131">**Odporúčané dokumenty**</span><span class="sxs-lookup"><span data-stu-id="4b6ff-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="4b6ff-132">Prenos vlastníctva predplatného Azure</span><span class="sxs-lookup"><span data-stu-id="4b6ff-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="4b6ff-133">Premiestnenie zdrojov do novej skupiny zdrojov alebo predplatného</span><span class="sxs-lookup"><span data-stu-id="4b6ff-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="4b6ff-134">Správa zdrojov pomocou služby Azure Portal</span><span class="sxs-lookup"><span data-stu-id="4b6ff-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
