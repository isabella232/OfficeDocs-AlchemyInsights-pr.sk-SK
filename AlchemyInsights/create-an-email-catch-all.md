---
title: Vytvoriť email chytiť všetky
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286306"
---
# <a name="create-an-email-catch-all"></a>Vytvoriť email chytiť všetky

Použitie úlovku všetko je silne odradiť. Je lepšie poskytnúť odskočiť späť odosielateľovi nájmu odosielateľom vedieť, že ich správa nemohla byť doručená, ako je určené, aby mohli podniknúť kroky. Môžete tiež obmedziť sledované poštovej schránky len chytiť predtým platné e-mailové adresy. 

Akékoľvek chytiť všetky schránky dostane veľa spamu a môže nakoniec vyplniť, ak nie pozorne sledovať. (Tam sú prijímacie limity.) 

Ak sa rozhodnete pokračovať, postupujte nasledovne:

1. Vytvorte dynamickú distribučnú skupinu & zahrnúť "všetky typy príjemcov."

2. Vytvoriť vyhradenú poštovú schránku zachytiť e-maily, napríklad catchall@domain.com.

3. Pre konkrétnu doménu, nastavte DomainType "InternalRelay". Ak neskôr odstránite úlovok všetky, uistite sa, že nastaviť doménu späť na autoritatívne.

4. Vytvoriť pravidlo prenosu Mailflow takto:

    - Ak je odosielateľ "mimo organizácie"
    - Presmerovanie správy na Catchall@domain.com
    - Okrem prípadov, keď je príjemca členom allusers@domain.com (distribučná skupina obsahuje všetkých členov)
    - Overte, či sa nové poštové schránky pridajú do dynamickej distribučnej skupiny
