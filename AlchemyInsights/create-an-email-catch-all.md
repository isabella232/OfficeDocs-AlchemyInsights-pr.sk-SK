---
title: Vytvorenie e-mailu na zachytenie všetkých
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816215"
---
# <a name="create-an-email-catch-all"></a>Vytvorenie e-mailu na zachytenie všetkých

Použitie všetkých záchytných údajov sa dôrazne neodporúča. Je lepšie vrátiť sa odosielateľovi, ktorý odosielateľovi dá vedieť, že sa ich správa nemôže doručiť ako adresa, aby mohol prijať opatrenia. Monitorovanú poštovú schránku môžete obmedziť iba na predtým platné e-mailové adresy. 

Každý úchylovok všetkých poštových schránok dostane veľa nevyžiadanej pošty a nakoniec sa môže vyplniť, ak nie je podrobne monitorovaný. (Prijímacie limity.) 

Ak sa rozhodnete pokračovať, postupujte takto:

1. Vytvorte dynamickú distribučnú skupinu& obsahuje položku Všetky typy príjemcov.

2. Vytvorte vyhradenú poštovú schránku na zachytenie e-mailov, napríklad catchall@domain.com.

3. Pre konkrétnu doménu nastavte položku DomainType na možnosť InternalRelay. Ak neskôr odstránite všetky, uistite sa, že ste doménu nastavili späť na možnosť Autoritatívny.

4. Pravidlo prenosu mailflow je možné vytvoriť takto:

    - Ak je odosielateľ "Mimo organizácie"
    - Presmerovať správu na Catchall@domain.com
    - Okrem prípadov, keď je príjemca členom člena allusers@domain.com (distribučná skupina obsahuje všetkých členov)
    - Overenie pridania nových poštových schránok do dynamickej distribučnej skupiny
