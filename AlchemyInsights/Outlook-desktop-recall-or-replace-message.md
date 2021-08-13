---
title: Outlook Odvolanie alebo nahradenie e-mailovej správy na pracovnej ploche
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918410"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Odvolanie alebo nahradenie Outlook-mailovej správy

- Ako správca môžete správy **v mene používateľov odvolať pomocou prostredia PowerShell.** V Centre spravovania nie je možné odvolať správy.
- Odvolať môžete **len správy odoslané ľuďom vo vašej organizácii.** Ak bola správa odoslaná napríklad na adresu služby Gmail, nemôžete ju odvolať.
- Odvolať môžete **len správy odoslané z Outlook 2016 z počítača**. Ak používateľ odošle správu pomocou Outlook pre Mac alebo Outlook na webe, nemôžete ju odvolať.

Odvolanie alebo nahradenie e-mailovej správy:

1. Na table priečinka na ľavej strane okna Outlook vyberte priečinok Odoslaná pošta.
1. Dvakrát kliknite na správu, ktorú chcete odvolať, a otvorte ju.
1. Vyberte kartu **Správa** a potom vyberte položku Akcie **odvolať**  >  **túto správu**.
1. Vyberte **položku Odstrániť neprečítané kópie tejto** správy alebo Odstrániť **neprečítané** kópie a nahradiť ich novou správou a potom vyberte tlačidlo **OK**.
1. Ak odosielate náhradnú správu, napíšte ju a potom vyberte položku **Odoslať**.
1. Úspech alebo neúspech odvolávania správy závisí od nastavení príjemcu v Outlook. Kroky na kontrolu odvolania nájdete v [tomto článku.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii

- Ak nie ste globálnym správcom, vaše konto je potrebné pridať do roly správcu eDiscovery alebo do roly správy vyhľadávania súladu, aby bolo možné vyhľadávať správy. Ak chcete odstrániť správy, musíte sa pripojiť k skupine rolí Správa organizácie alebo k role správy vyhľadávania a vymazania. Povolenia týchto rolí sa priraďujú v [Centre zabezpečenia a dodržiavania súladu.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Vytvorte vyhľadávanie obsahu a](https://docs.microsoft.com/microsoft-365/compliance/content-search) vyhľadajte správu na odstránenie.
- [Pripojenie do Centra zabezpečenia a dodržiavania súladu prostredia PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Ak používate viacfaktorové overovanie, pozrite si Pripojenie do Microsoft 365 zabezpečenia a dodržiavania súladu [prostredia PowerShell pomocou viacfaktorového overovania.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)