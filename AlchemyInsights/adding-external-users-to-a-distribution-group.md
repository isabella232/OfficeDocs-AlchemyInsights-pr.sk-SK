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
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934848"
---
# <a name="add-external-users-to-a-distribution-group"></a>Pridanie externých používateľov do distribučnej skupiny

Pridanie externého kontaktu do distribučnej skupiny (DS) má dva kroky:
  
1. Vytvorenie poštového kontaktu pre externého používateľa:
    
    1. V centre spravovania prejdite na **stránku Kontakty**  >  [](https://admin.microsoft.com/adminportal/home#/Contact) používateľov. 
    
    2. Vyberte **položku Pridať kontakt**.
    
    3. Zadajte informácie o kontakte a vyberte položku **Pridať**.
    
2. Pridanie poštového kontaktu do skupiny pre vaše oddelenie nevyžiadanej pošty:
    
    1. V centre spravovania prejdite na **stránku**  >  [Skupiny.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Nájdite VD, ku ktorej chcete pridať externého používateľa, a vyberte ju, aby sa otvorilo dialógové okno úprav.
    
    3. Na karte **Členovia** vyberte položku Zobraziť **všetkých a spravovať členov**. 
    
    4. Vyberte **položku Pridať členov**.
    
    5. Vyberte poštový kontakt, ktorý ste vytvorili v predchádzajúcom kroku, a potom vyberte položku **Uložiť**.
    
Ak po týchto krokoch externí používatelia nemohli odosielať e-maily alebo od nich prijímať e-maily, môže to byť preto, že v VS je označené tak, aby umožňovali e-maily iba od interných používateľov. Toto nastavenie môžete skontrolovať a opraviť podľa pokynov [uvedených tu.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Poznámka:** Tieto pokyny nie sú platiť, ak je typ skupiny "Microsoft 365 skupina" namiesto "Distribučná skupina". V takom prípade môžete pridať externého používateľa priamo do skupiny z Outlook. Podrobné informácie o Microsoft 365 skupiny, ako aj pokyny na pridávanie externých hostí, nájdete v [tomto článku.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  