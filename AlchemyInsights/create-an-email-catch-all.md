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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080761"
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
