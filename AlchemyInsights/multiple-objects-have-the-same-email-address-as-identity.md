---
title: Viaceré objekty majú rovnakú e-mailovú adresu ako identita
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439711"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Viaceré objekty majú rovnakú e-mailovú adresu ako identita

**Viaceré objekty**

Jedným z bežných dôvodov tejto chyby nie je možné správne smerovať požiadavku služby Outlook Web Access v prítomnosti viacerých objektov s rovnakou e-mailovú adresu ako identita. Ak chcete nájsť tieto objekty, spustite nasledujúce príkazy:

· Získať príjemcu<email address>

· Získať používateľa<email address>

· Získajte užívateľa <email address> -SoftDeletedUser

· Získať kontakt<email address>

· Získať poštovej <email address> schránky - PublicFolder

· Získať poštovej <email address> schránky - IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Ak chcete vyriešiť tento problém, odstráňte viaceré objekty s rovnakou e-mailovú identitu a uistite sa, že existuje jeden objekt s konkrétnou e-mailovú identitu a že jeho typ príjemcu je UserMailbox.

**Rovnaká adresa sa používa pre obchodné a spotrebiteľské poštové schránky**

Ďalšou príčinou je, keď sa rovnaká adresa používa pre obchodné a spotrebiteľské poštové schránky. V tomto prípade musí používateľ zmeniť svoj primárny spotrebiteľský alias, kým Cafe podporuje tento scenár. Ide o trvalú chybu, ktorá nezmizne bez zásahu.

Podrobnosti nájdete v téme [Zmena e-mailovej adresy alebo telefónneho čísla konta Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).