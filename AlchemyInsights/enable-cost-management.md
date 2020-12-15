---
title: Povolenie správy nákladov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678771"
---
# <a name="enable-cost-management"></a><span data-ttu-id="26836-102">Povolenie správy nákladov</span><span class="sxs-lookup"><span data-stu-id="26836-102">Enable cost management</span></span>

<span data-ttu-id="26836-103">**Čo znamená, že náklady sú pre vašu organizáciu vypnuté?**</span><span class="sxs-lookup"><span data-stu-id="26836-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="26836-104">Organizácie, ktoré používajú kontá Enterprise Agreement (EA) alebo Microsoft Customer Agreement (MCA), môžu zablokovať prístup k informáciám o nákladoch a informáciám o cenách.</span><span class="sxs-lookup"><span data-stu-id="26836-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="26836-105">Po prihlasovaní na portál Azure môžete použiť fakturačné rozhrania API na programovanie faktúr (raz sa prihlásili) a Podrobnosti o používaní.</span><span class="sxs-lookup"><span data-stu-id="26836-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="26836-106">**Povolenie ďalších používateľov na prístup k faktúram**</span><span class="sxs-lookup"><span data-stu-id="26836-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="26836-107">Prejdite na položky **predplatné Blade** na portáli Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="26836-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="26836-108">Vyberte položku **faktúry** a potom **prístup k faktúram**.</span><span class="sxs-lookup"><span data-stu-id="26836-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="26836-109">Zapnite Access a potom uložte zmeny a umožnite používateľom v rámci úloh v rámci predplatného preberať faktúry.</span><span class="sxs-lookup"><span data-stu-id="26836-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="26836-110">Správca konta môže tiež nakonfigurovať, aby sa faktúry odosielali e-mailom.</span><span class="sxs-lookup"><span data-stu-id="26836-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="26836-111">Ďalšie informácie nájdete v téme [získanie faktúry prostredníctvom e-mailu](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="26836-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="26836-112">**Pridanie používateľov do roly čítačky fakturácie**</span><span class="sxs-lookup"><span data-stu-id="26836-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="26836-113">Prejdite na položky **predplatné Blade** na portáli Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="26836-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="26836-114">Vyberte položku **Access Control (IAM)** a potom kliknite na položku **Pridať**.</span><span class="sxs-lookup"><span data-stu-id="26836-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="26836-115">Vyberte položku **čítačka fakturácie** na stránke **Vyberte rolu** .</span><span class="sxs-lookup"><span data-stu-id="26836-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="26836-116">Zadajte e-mailovú adresu používateľa, ktorého chcete pozvať, a potom kliknite na **tlačidlo OK** , ak chcete pozvánku Odoslať.</span><span class="sxs-lookup"><span data-stu-id="26836-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="26836-117">Ak sa chcete prihlásiť ako čítačka fakturácie, postupujte podľa pokynov uvedených v časti pozvať e-mail.</span><span class="sxs-lookup"><span data-stu-id="26836-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="26836-118">Ďalšie informácie nájdete v téme [udelenie prístupu k fakturácii](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="26836-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="26836-119">**Odporúčané dokumenty**</span><span class="sxs-lookup"><span data-stu-id="26836-119">**Recommended documents**</span></span>

- [<span data-ttu-id="26836-120">Povolenie zobrazenia DA a AO cez portál EA</span><span class="sxs-lookup"><span data-stu-id="26836-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="26836-121">Náklady zahrnuté v správe nákladov</span><span class="sxs-lookup"><span data-stu-id="26836-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="26836-122">Podporované ponuky služby Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="26836-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="26836-123">Revízia nákladov na analýzu nákladov</span><span class="sxs-lookup"><span data-stu-id="26836-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="26836-124">Poskytnutie prístupu k informáciám o fakturácii</span><span class="sxs-lookup"><span data-stu-id="26836-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="26836-125">Kontrola prístupu k Zmluve o zákazníkovi spoločnosti Microsoft</span><span class="sxs-lookup"><span data-stu-id="26836-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






