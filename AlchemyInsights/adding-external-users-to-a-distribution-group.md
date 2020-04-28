---
title: Pridanie externých používateľov do distribučnej skupiny
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910947"
---
# <a name="add-external-users-to-a-distribution-group"></a>Pridanie externých používateľov do distribučnej skupiny

Pridanie externého kontaktu do distribučnej skupiny (DG) je dvojfázový proces:
  
1. Vytvorenie poštového kontaktu pre externého používateľa:
    
    1. V centre spravovania prejdite na stránku **Používatelia** > [kontaktov](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Vyberte položku **Pridať kontakt**.
    
    3. Zadajte informácie o kontakte a vyberte položku **Pridať**.
    
2. Pridajte poštový kontakt do svojho GR:
    
    1. V centre spravovania prejdite na[Groups](https://admin.microsoft.com/adminportal/home#/groups)  >  **stránku skupiny skupín**. 
    
    2. Nájdite GR, do ktorého chcete pridať externého používateľa, a vyberte ho, ak chcete otvoriť dialógové okno úprav.
    
    3. Na karte **členovia** vyberte položku **Zobraziť všetky a spravovať členov**. 
    
    4. Vyberte položku **pridať členov**.
    
    5. Vyberte poštový kontakt, ktorý ste vytvorili v predchádzajúcom kroku, a potom vyberte položku **Uložiť**.
    
Ak po týchto krokoch Externí používatelia nemôžu odosielať e-maily do GR alebo neprijímajú e-maily z nej, mohlo by to byť, že GR je označené, že povolí iba e-maily od interných používateľov. Môžete skontrolovať túto konfiguráciu a opraviť ju podľa návodu [tu](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Poznámka:** Tieto pokyny neplatia, ak typ skupiny je "Microsoft 365 skupina" namiesto "distribučnej skupiny." V takom prípade môžete externý používateľ pridať priamo do skupiny z programu Outlook. Podrobné informácie o Microsoft 365 skupiny hostí, rovnako ako návod na pridávanie externých hostí možno nájsť v [tomto článku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  