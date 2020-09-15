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
# <a name="add-external-users-to-a-distribution-group"></a>Pridanie externých používateľov do distribučnej skupiny

Pridanie externého kontaktu do distribučnej skupiny (DG) je dvojstupňový proces:
  
1. Vytvorenie poštového kontaktu pre externého používateľa:
    
    1. V centre spravovania prejdite na stránku kontakty **používateľov**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Vyberte položku **Pridať kontakt**.
    
    3. Zadajte informácie o kontakte a vyberte položku **Pridať**.
    
2. Pridanie poštového kontaktu do GR:
    
    1. V centre spravovania prejdite na stránku skupiny **skupín**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Vyhľadajte GR, do ktorého chcete pridať externého používateľa, a vyberte ho, čím sa otvorí dialógové okno Upraviť.
    
    3. Na karte **členovia** vyberte položku **Zobraziť všetky a spravovať členov**. 
    
    4. Vyberte položku **pridať členov**.
    
    5. Vyberte poštový kontakt, ktorý ste vytvorili v predchádzajúcom kroku, a potom vyberte položku **Uložiť**.
    
Ak sa po vykonaní týchto krokov nebudú môcť Externí používatelia odosielať e-maily generálnemu riaditeľstvu alebo neprijímajú e-maily z neho, môže sa stať, že Generálne riaditeľstvo povoľuje iba e-maily od interných používateľov. Môžete skontrolovať túto konfiguráciu a opraviť ju podľa pokynov uvedených [nižšie](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Poznámka:** Tieto pokyny sa neuplatnia, ak je typ skupiny "skupina Microsoft 365" namiesto časti "distribučná skupina". Ak ide o tento prípad, externý používateľ môžete pridať priamo do skupiny z Outlooku. Podrobné informácie o skupinách v službách Microsoft 365, ako aj pokyny na pridávanie externých hostí, nájdete v [tomto článku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  