---
title: Modern Azure email invoicing
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820841"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="04d7f-102">E-mailová fakturácia v Azure</span><span class="sxs-lookup"><span data-stu-id="04d7f-102">Email invoicing in Azure</span></span>

<span data-ttu-id="04d7f-103">Ak chcete aktualizovať predvoľby e-mailovej faktúry, musíte mať v fakturačnom profile alebo svojom fakturačnom konte rolu vlastníka alebo prispievateľa.</span><span class="sxs-lookup"><span data-stu-id="04d7f-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="04d7f-104">Keď sa prihlásite, všetci používatelia s vlastníkom, prispievateľom, čitateľmi a rolami správcu faktúr vo fakturačnom profile budú faktúru odoslať e-mailom.</span><span class="sxs-lookup"><span data-stu-id="04d7f-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="04d7f-105">Prihláste sa na [portál Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="04d7f-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="04d7f-106">Vyhľadajte **Cost Management + Billing** (Správa nákladov a fakturácia).</span><span class="sxs-lookup"><span data-stu-id="04d7f-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="04d7f-107">Na **ľavej strane** vyberte položku Faktúry a potom v **hornej** časti stránky vyberte položku E-mailová faktúra.</span><span class="sxs-lookup"><span data-stu-id="04d7f-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="04d7f-108">Ak máte viacero fakturačných profilov, vyberte fakturačný profil a potom vyberte položku **Prihlásiť sa**.</span><span class="sxs-lookup"><span data-stu-id="04d7f-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="04d7f-109">Vyberte **položku Aktualizovať**.</span><span class="sxs-lookup"><span data-stu-id="04d7f-109">Select **Update**.</span></span>
6. <span data-ttu-id="04d7f-110">Ak máte viacero fakturačných profilov, vyberte fakturačný profil a potom vyberte položku **Prihlásiť sa**.</span><span class="sxs-lookup"><span data-stu-id="04d7f-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="04d7f-111">Ostatným používateľom poskytnete prístup na zobrazenie, stiahnutie a účtovanie, a to tak, že im priradíte rolu správcu faktúr pre fakturačný profil spoločnosti MCA alebo MPA.</span><span class="sxs-lookup"><span data-stu-id="04d7f-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="04d7f-112">Ak ste sa rozhodli dostať faktúru e-mailom, používatelia tiež dostane faktúry e-mailom.</span><span class="sxs-lookup"><span data-stu-id="04d7f-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="04d7f-113">Prihláste sa na [portál Azure.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="04d7f-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="04d7f-114">Vyhľadajte **Cost Management + Billing** (Správa nákladov a fakturácia).</span><span class="sxs-lookup"><span data-stu-id="04d7f-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="04d7f-115">Na **ľavej** strane vyberte položku Fakturačné profily.</span><span class="sxs-lookup"><span data-stu-id="04d7f-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="04d7f-116">Zo zoznamu fakturačných profilov vyberte fakturačný profil, ku ktorému chcete priradiť rolu správcu faktúr.</span><span class="sxs-lookup"><span data-stu-id="04d7f-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="04d7f-117">Na ľavej strane vyberte položku Access **Control (IAM)** a potom v **hornej** časti stránky vyberte položku Pridať.</span><span class="sxs-lookup"><span data-stu-id="04d7f-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="04d7f-118">V rozbaľovacom zozname Rola vyberte položku **Správca faktúr**.</span><span class="sxs-lookup"><span data-stu-id="04d7f-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="04d7f-119">Zadajte e-mailovú adresu používateľa, ktorý má prístup poskytnúť.</span><span class="sxs-lookup"><span data-stu-id="04d7f-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="04d7f-120">Ak **chcete priradiť rolu,** vyberte položku Uložiť.</span><span class="sxs-lookup"><span data-stu-id="04d7f-120">Select **Save** to assign the role.</span></span>
