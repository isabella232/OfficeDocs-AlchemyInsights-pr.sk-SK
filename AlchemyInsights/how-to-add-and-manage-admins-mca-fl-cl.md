---
title: Ako pridať a spravovať správcov
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
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755526"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="d16de-102">Ako pridať a spravovať správcov</span><span class="sxs-lookup"><span data-stu-id="d16de-102">How to add and manage admins</span></span>

<span data-ttu-id="d16de-103">Na základe popisu problému sme našli riešenie.</span><span class="sxs-lookup"><span data-stu-id="d16de-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="d16de-104">Väčšina zákazníkov si po vykonaní našej dokumentácie dokázala vyriešiť svoj problém sami.</span><span class="sxs-lookup"><span data-stu-id="d16de-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="d16de-105">Ak chcete spravovať fakturačné konto pre zmluvu o zákazníkovi spoločnosti Microsoft (MCA), môžete použiť rôzne roly s požadovanou úrovňou prístupu.</span><span class="sxs-lookup"><span data-stu-id="d16de-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="d16de-106">Tieto roly dopĺňajú vstavané roly služby Azure, ktoré vám pomôžu ovládať zdroje.</span><span class="sxs-lookup"><span data-stu-id="d16de-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="d16de-107">**Ak chcete pridať úlohy fakturácie na portáli Azure:**</span><span class="sxs-lookup"><span data-stu-id="d16de-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="d16de-108">Prihláste sa na [portáli Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="d16de-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="d16de-109">Vyhľadajte *správu nákladov + Fakturácia*.</span><span class="sxs-lookup"><span data-stu-id="d16de-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="d16de-110">Vyberte položku Access Control (IAM) v rozsahu, akým je napríklad fakturačné konto, profil fakturácie alebo sekcia fakturácia, do ktorej chcete poskytnúť prístup.</span><span class="sxs-lookup"><span data-stu-id="d16de-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="d16de-111">Stránka Access Control (IAM) uvádza používateľov a skupiny, ktoré sú priradené ku každej úlohe daného rozsahu.</span><span class="sxs-lookup"><span data-stu-id="d16de-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="d16de-112">Ak chcete používateľovi poskytnúť prístup, vyberte položku **Pridať** v hornej časti stránky.</span><span class="sxs-lookup"><span data-stu-id="d16de-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="d16de-113">V rozbaľovacom zozname *rola* vyberte rolu.</span><span class="sxs-lookup"><span data-stu-id="d16de-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="d16de-114">Zadajte e-mailovú adresu používateľa, ktorému chcete poskytnúť prístup.</span><span class="sxs-lookup"><span data-stu-id="d16de-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="d16de-115">Ak chcete rolu priradiť, vyberte položku **Uložiť** .</span><span class="sxs-lookup"><span data-stu-id="d16de-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="d16de-116">Ak chcete odstrániť prístup pre používateľa, vyberte používateľa s priradením roly, ktorú chcete odstrániť.</span><span class="sxs-lookup"><span data-stu-id="d16de-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="d16de-117">Vyberte položku **odstrániť**.</span><span class="sxs-lookup"><span data-stu-id="d16de-117">Select **Remove**.</span></span>

<span data-ttu-id="d16de-118">**Odporučené dokumenty**</span><span class="sxs-lookup"><span data-stu-id="d16de-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="d16de-119">Definície roly fakturácie</span><span class="sxs-lookup"><span data-stu-id="d16de-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="d16de-120">Roly a úlohy konta fakturácie</span><span class="sxs-lookup"><span data-stu-id="d16de-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="d16de-121">Začíname s fakturačným kontom MCA</span><span class="sxs-lookup"><span data-stu-id="d16de-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="d16de-122">Kontrola prístupu k Zmluve o zákazníkovi spoločnosti Microsoft</span><span class="sxs-lookup"><span data-stu-id="d16de-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
