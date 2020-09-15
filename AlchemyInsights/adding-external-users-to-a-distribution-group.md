---
title: Pridanie externých používateľov do distribučnej skupiny
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663528"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="4b273-102">Pridanie externých používateľov do distribučnej skupiny</span><span class="sxs-lookup"><span data-stu-id="4b273-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="4b273-103">Pridanie externého kontaktu do distribučnej skupiny (DG) je dvojstupňový proces:</span><span class="sxs-lookup"><span data-stu-id="4b273-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="4b273-104">Vytvorenie poštového kontaktu pre externého používateľa:</span><span class="sxs-lookup"><span data-stu-id="4b273-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="4b273-105">V centre spravovania prejdite na stránku kontakty **používateľov**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="4b273-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="4b273-106">Vyberte položku **Pridať kontakt**.</span><span class="sxs-lookup"><span data-stu-id="4b273-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="4b273-107">Zadajte informácie o kontakte a vyberte položku **Pridať**.</span><span class="sxs-lookup"><span data-stu-id="4b273-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="4b273-108">Pridanie poštového kontaktu do GR:</span><span class="sxs-lookup"><span data-stu-id="4b273-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="4b273-109">V centre spravovania prejdite na stránku skupiny **skupín**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="4b273-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="4b273-110">Vyhľadajte GR, do ktorého chcete pridať externého používateľa, a vyberte ho, čím sa otvorí dialógové okno Upraviť.</span><span class="sxs-lookup"><span data-stu-id="4b273-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="4b273-111">Na karte **členovia** vyberte položku **Zobraziť všetky a spravovať členov**.</span><span class="sxs-lookup"><span data-stu-id="4b273-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="4b273-112">Vyberte položku **pridať členov**.</span><span class="sxs-lookup"><span data-stu-id="4b273-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="4b273-113">Vyberte poštový kontakt, ktorý ste vytvorili v predchádzajúcom kroku, a potom vyberte položku **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="4b273-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="4b273-114">Ak sa po vykonaní týchto krokov nebudú môcť Externí používatelia odosielať e-maily generálnemu riaditeľstvu alebo neprijímajú e-maily z neho, môže sa stať, že Generálne riaditeľstvo povoľuje iba e-maily od interných používateľov.</span><span class="sxs-lookup"><span data-stu-id="4b273-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="4b273-115">Môžete skontrolovať túto konfiguráciu a opraviť ju podľa pokynov uvedených [nižšie](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="4b273-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="4b273-116">**Poznámka:** Tieto pokyny sa neuplatnia, ak je typ skupiny "skupina Microsoft 365" namiesto časti "distribučná skupina".</span><span class="sxs-lookup"><span data-stu-id="4b273-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="4b273-117">Ak ide o tento prípad, externý používateľ môžete pridať priamo do skupiny z Outlooku.</span><span class="sxs-lookup"><span data-stu-id="4b273-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="4b273-118">Podrobné informácie o skupinách v službách Microsoft 365, ako aj pokyny na pridávanie externých hostí, nájdete v [tomto článku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="4b273-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  