---
title: Moderná Fakturácia e-mailov v službe Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922143"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="67b11-102">Fakturácia e-mailu v službe Azure</span><span class="sxs-lookup"><span data-stu-id="67b11-102">Email invoicing in Azure</span></span>

<span data-ttu-id="67b11-103">Ak chcete aktualizovať svoju preferovanú e-mailovú faktúru, musíte mať vlastníka alebo rolu prispievateľa v profile fakturácie alebo v jeho fakturačnom konte.</span><span class="sxs-lookup"><span data-stu-id="67b11-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="67b11-104">Po prihlásení sa všetci používatelia s rolami vlastníka, prispievateľa, čítačky a správca faktúry v profile fakturácie dostanú do e-mailu svoju faktúru.</span><span class="sxs-lookup"><span data-stu-id="67b11-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="67b11-105">Prihláste sa na [portáli Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="67b11-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="67b11-106">Vyhľadajte **správu nákladov + Fakturácia**.</span><span class="sxs-lookup"><span data-stu-id="67b11-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="67b11-107">Vyberte položku **faktúry** na ľavej strane a potom vyberte položku **e-mailová faktúra** v hornej časti stránky.</span><span class="sxs-lookup"><span data-stu-id="67b11-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="67b11-108">Ak máte viacero profilov fakturácie, vyberte profil fakturácie a potom vyberte položku **opt in (prihlásiť** sa).</span><span class="sxs-lookup"><span data-stu-id="67b11-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="67b11-109">Vyberte položku **aktualizovať**.</span><span class="sxs-lookup"><span data-stu-id="67b11-109">Select **Update**.</span></span>
6. <span data-ttu-id="67b11-110">Ak máte viacero profilov fakturácie, vyberte profil fakturácie a potom vyberte položku **opt in (prihlásiť** sa).</span><span class="sxs-lookup"><span data-stu-id="67b11-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="67b11-111">Ostatným používateľom povolíte prístup na zobrazenie, stiahnutie a platenie faktúr priradením roly správcu fakturácie pre profil fakturácie MCA alebo MPA.</span><span class="sxs-lookup"><span data-stu-id="67b11-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="67b11-112">Ak ste sa rozhodli dostať svoju faktúru e-mailom, používatelia dostanú faktúry aj e-mailom.</span><span class="sxs-lookup"><span data-stu-id="67b11-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="67b11-113">Prihláste sa na [portáli Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="67b11-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="67b11-114">Vyhľadajte **správu nákladov + Fakturácia**.</span><span class="sxs-lookup"><span data-stu-id="67b11-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="67b11-115">Vyberte položku **profily fakturácie** na ľavej strane.</span><span class="sxs-lookup"><span data-stu-id="67b11-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="67b11-116">V zozname profily fakturácie vyberte profil fakturácie, ku ktorému chcete priradiť rolu správcu faktúry.</span><span class="sxs-lookup"><span data-stu-id="67b11-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="67b11-117">Vyberte položku **Access Control (IAM)** na ľavej strane a potom vyberte položku **Pridať** v hornej časti stránky.</span><span class="sxs-lookup"><span data-stu-id="67b11-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="67b11-118">V rozbaľovacom zozname rola vyberte položku **Správca fakturácie**.</span><span class="sxs-lookup"><span data-stu-id="67b11-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="67b11-119">Zadajte e-mailovú adresu používateľa, ktorému chcete poskytnúť prístup.</span><span class="sxs-lookup"><span data-stu-id="67b11-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="67b11-120">Ak chcete rolu priradiť, vyberte položku **Uložiť** .</span><span class="sxs-lookup"><span data-stu-id="67b11-120">Select **Save** to assign the role.</span></span>
