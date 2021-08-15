---
title: Konfigurácia služby poskytovania
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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033293"
---
# <a name="configuring-the-provision-service"></a>Konfigurácia služby poskytovania

Na to, aby automatizovaný používateľ používal funkcie poskytovania služieb, Azure AD vyžaduje platné poverenia, ktoré jej umožňujú pripojiť sa k rozhraniu API webových služieb Workday. Ďalej sa tlačidlo Testovať pripojenie v pracovnom dni k aplikácii ad User Provisioning overí aj vtedy, ak sa dokáže pripojiť k službe Azure AD Pripojenie Provisioning Agenta priradenému k doméne AD.

Ak portál Azure vracia pri ukladaní poverení chybu, postupujte podľa odporúčaných krokov uvedených nižšie:

1. Skontrolujte, či ste nakonfigurovali používateľské konto systému integrácie Pracovného dňa, ako sa uvádza v sekcii kurzu Konfigurácia používateľa systému integrácie [v pracovný deň.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Skontrolujte, či je služba Azure AD Pripojenie Provisioning Agent Service spustená na lokálnom Windows pomocou konzoly Services Management Console. Stav agenta môžete skontrolovať aj na portáli Azure kliknutím na tlačidlo Zobraziť lokálnych agentov.
3. Skontrolujte, či zadávate hodnotu pre pole Pracovný deň meno používateľa pomocou formátu username@workday-meno nájomníka. Ak chýba názov pracovného dňa-nájomníka, overenie pracovného dňa zlyhá.
4. Ak konfigurujete integráciu s nájomníkom na implementáciu pracovného dňa, poznačte si plánované hodiny prestojov nájomníka pracovného dňa. Pracovný deň naplánuje pre nájomníkov s implementácii cez víkendy (zvyčajne od piatka do soboty rána) a zlyhania pripojenia počas tohto okna výpadku je známym problémom, ktorý sa automaticky vyrieši, keď sa nájomníci na implementáciu vrátia do režimu online.
5. V zriedkavých prípadoch sa môže zobraziť aj táto chyba, ak sa heslo používateľa systému integrácie zmenilo z dôvodu obnovenia nájomníka alebo ak je konto zamknuté alebo ak vypršala jeho platnosť. Skontrolujte stav používateľa systému integrácie so správcom pracovného dňa.

Ďalšie podrobnosti o konfigurácii pracovného dňa na automatické poskytovanie údajov nájdete v [kurze: Konfigurácia pracovného dňa pre automatické poskytovanie služieb používateľom.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
