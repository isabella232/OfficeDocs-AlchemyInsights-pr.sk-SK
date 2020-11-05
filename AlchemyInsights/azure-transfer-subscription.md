---
title: Prenos vlastníctva služby Azure fakturácie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922169"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="93941-102">Prenos vlastníctva služby Azure fakturácie</span><span class="sxs-lookup"><span data-stu-id="93941-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="93941-103">Prihláste sa na [portáli Azure](https://portal.azure.com/) ako správca konta na fakturáciu s predplatným, ktoré chcete preniesť.</span><span class="sxs-lookup"><span data-stu-id="93941-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="93941-104">Ak si nie ste istí, či ste a ste správcom, alebo ak potrebujete zistiť, kto je, pozrite si tému [určenie správcu fakturácie konta](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="93941-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="93941-105">Vyhľadávanie v **správe nákladov + Fakturácia**.</span><span class="sxs-lookup"><span data-stu-id="93941-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="93941-106">Vyberte položku **predplatné** z ľavej tably.</span><span class="sxs-lookup"><span data-stu-id="93941-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="93941-107">V závislosti od Accessu možno budete musieť vybrať rozsah fakturácie a potom **predplatné** alebo **predplatné Azure**.</span><span class="sxs-lookup"><span data-stu-id="93941-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="93941-108">Vyberte položku **previesť vlastníctvo fakturácie** na predplatné, ktoré chcete preniesť</span><span class="sxs-lookup"><span data-stu-id="93941-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="93941-109">Zadajte e-mailovú adresu používateľa, ktorý je správcom fakturácie konta, ktorý bude novým vlastníkom predplatného a potom vyberte položku **Odoslať žiadosť o prenos** .</span><span class="sxs-lookup"><span data-stu-id="93941-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="93941-110">Používateľ dostane e-mail s pokynmi na kontrolu žiadosti o prenos.</span><span class="sxs-lookup"><span data-stu-id="93941-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="93941-111">Ak chcete schváliť žiadosť o prenos, používateľ vyberie prepojenie v e-maile a postupujte podľa pokynov.</span><span class="sxs-lookup"><span data-stu-id="93941-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="93941-112">**Poznámka** : Ak prenesiete vlastníctvo fakturácie vášho predplatného na konto používateľa v inom nájomníkovi služby Azure AD, všetky priradenia [riadenia prístupu na základe rolí (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)na spravovanie zdrojov v predplatnom sa natrvalo odstránia.</span><span class="sxs-lookup"><span data-stu-id="93941-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="93941-113">Iba nový vlastník bude mať prístup k správe zdrojov v predplatnom.</span><span class="sxs-lookup"><span data-stu-id="93941-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="93941-114">Ďalšie informácie nájdete v téme [prenos predplatného používateľovi v inom nájomníkovi služby Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="93941-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="93941-115">**Odporúčané dokumenty**</span><span class="sxs-lookup"><span data-stu-id="93941-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="93941-116">Prenos vlastníctva fakturácie prostredníctvom Azure predplatného na iné konto</span><span class="sxs-lookup"><span data-stu-id="93941-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="93941-117">Informácie o prenose vlastníctva fakturácie pre predplatné Azure</span><span class="sxs-lookup"><span data-stu-id="93941-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="93941-118">Prenos Visual Studio, Microsoft Partner Network (MPN) a Pay as you go dev/test predplatného</span><span class="sxs-lookup"><span data-stu-id="93941-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="93941-119">Najčastejšie otázky o prenose vlastníctva</span><span class="sxs-lookup"><span data-stu-id="93941-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="93941-120">Riešenie problémov s vlastníctvom prenosu</span><span class="sxs-lookup"><span data-stu-id="93941-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
