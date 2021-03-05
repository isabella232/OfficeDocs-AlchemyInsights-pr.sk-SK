---
title: Konfigurovanie služby zabezpečenia
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484043"
---
# <a name="configuring-the-provision-service"></a>Konfigurovanie služby zabezpečenia

Ak chcete, aby automatizované poskytovanie používateľov fungovalo, Azure AD vyžaduje platné poverenia, ktoré mu umožnia pripojiť sa k službe API pre webové služby v rámci pracovného dňa. Okrem toho sa v aplikácii na poskytovanie služby AD User (skúšobné pripojenie) na stránke pracovný postup overí aj to, či sa používateľ môže pripojiť k agentovi poskytovania služby Azure AD Connect, ktorý je priradený k REKLAMnej doméne.

Ak Azure Portal vráti chybu pri ukladaní poverení, postupujte podľa nižšie uvedených odporúčaných krokov:

1. Potvrďte, že ste nakonfigurovali používateľské konto na integráciu do pracovného dňa, ako je to uvedené v časti výučba v časti [Konfigurácia používateľa systému integrácie v deň](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Overte, či je služba Azure AD Connect poskytovanie agenta na lokálnom serveri Windowsu spustená pomocou konzoly na správu služieb. Môžete tiež skontrolovať stav agenta na portáli Azure kliknutím na tlačidlo Zobraziť lokálne agentov.
3. Uistite sa, že zadávate hodnotu pre pole meno používateľa v textovom poli s použitím formátu username@workday – meno nájomníka. Ak pracovný deň – nájomník – meno chýba, zlyhá overenie pracovného dňa.
4. Ak konfigurujete integráciu s nájomníkom vykonávania pracovného dňa, zaznamenajte si plánované prestoje v pracovnom čase nájomníka. Pracovný deň naplánoval časový úsek pre svojich nájomníkov v priebehu víkendov (zvyčajne z piatku večer do soboty ráno) a zlyhanie pripojenia počas tohto časového obdobia je známy problém, ktorý sa automaticky vyrieši, hneď ako budú nájomníki implementácie naspäť online.
5. V zriedkavých prípadoch sa môže táto chyba Zobraziť aj v prípade, že sa heslo používateľa systému integrácie zmenilo z dôvodu obnovenia nájomníka alebo ak je konto v stave uzamknutia alebo skončenia platnosti. Skontrolujte stav používateľa systému integrácie s správcom pracovného dňa.

Ďalšie informácie o konfigurácii pracovného dňa na automatické poskytovanie informácií nájdete v téme [kurz: Konfigurácia pracovného dňa na automatické poskytovanie používateľov](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
