---
title: Vytvorenie e-mailového úlovku všetkých
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713001"
---
# <a name="create-an-email-catch-all"></a>Vytvorenie e-mailového úlovku všetkých

Používanie všetkých úlovkov je silne odradzované. Je lepšie poskytnúť odskočiť späť odosielateľovi, ktorí odosielajú odosielateľovi, že ich správa sa nedá dodať ako adresovaná, aby mohli konať. Môžete tiež obmedziť sledovanú poštovú schránku, aby sa len chytiť predtým platné e-mailové adresy. 

Akýkoľvek úlovok všetky poštovej schránky dostane veľa nevyžiadanej pošty a môže nakoniec vyplniť, ak nie pozorne sledovať. (Dostávajú sa limity.) 

Ak sa rozhodnete pokračovať, postupujte takto:

1. Vytvorenie dynamickej distribučnej skupiny & zahrnúť všetky typy príjemcov.

2. Vytvorte vyhradenú poštovú schránku na zachytenie e-mailov, napríklad catchall@domain.com.

3. Pre konkrétnu doménu nastavte DomainType na "InternalRelay". Ak neskôr odstránite všetky úlovky, nezabudnite nastaviť doménu späť na autoritatívne.

4. Vytvorte pravidlo prenosu Poštyhttps://Configure.Office.com/scenario.aspx?sid=12 takto:

    - Ak sa odosielateľ nachádza mimo organizácie
    - Presmerovať správu na Catchall@domain.com
    - Okrem prípadov, keď je príjemca členom allusers@domain.com (distribučná skupina obsahuje všetkých členov)
    - Overenie pridávania nových poštových schránok do dynamickej distribučnej skupiny
