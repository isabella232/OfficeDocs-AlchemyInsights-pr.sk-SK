---
title: Predvolené Outlook označenia údajov sa použilo
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455087"
---
# <a name="default-outlook-label-setting-not-applied"></a>Predvolené Outlook označenia údajov sa použilo

Ak sa vaše predvolené nastavenia označenia na lokalite Outlook neudejú správne a použije sa iné označenie alebo sa na vás u vás nič nepoznanie, môže sa vyskytol známy problém (MC277818) a na vyriešenie problému by ste mali použiť jednu z týchto 2 možností:

**1. možnosť:**

1. Prejdite do centra Microsoft 365 Compliance Center >  >  **Solutions Information Protection**.
1. Vyberte **položku Politiky** menoviek a vyberte politiku označenia, ktorú chcete upraviť **(Nastavenie služby OutlookDefaultlabel** nie je správne nastavené na správnom nastavení s otázkou politiky označenia. Ak **chcete zobraziť toto nastavenie, spustite get-labelpolicy** a potom vyberte položku Upraviť **politiku**.
1. Výberom položky **Ďalej** zobrazte nastavenie Použiť toto predvolené označenie na e-maily **,** ktoré je k dispozícii, ak vyberiete možnosť Vyžadovať použitie označenia na e-maily a dokumenty v **heir** aj v dialógovom okne **Nastavenie** politiky.
1. V **dialógovom okne Použiť predvolené označenie na** dokumenty vyberte z **rozbaľovacieho** zoznamu položku Žiadne.
1. Nastavenia **označení uložíte** **výberom** položky Ďalej a Odoslať.

**2. možnosť:**

V [prostredí Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)Centra zabezpečenia a dodržiavania súladu Set-LabelPolicy príkazového riadka  programu **OutlookDefaultlabel** na možnosť Žiadne v časti {OutlookDefaultLabel="None"}.

Spustenie: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Ďalšie informácie o predvolených označeniach pre Outlook nájdete v téme [Nastavenie iného predvoleného Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)