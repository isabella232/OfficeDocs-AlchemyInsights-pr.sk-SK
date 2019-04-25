---
title: Desktop odvolanie správy programu Outlook alebo nahradiť e-mailovej správy
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389778"
---
# <a name="recall-or-replace-an-email-message"></a>Odvolanie alebo nahradenie e-mailovej správy

- Ako admin, môžete **pripomenúť správy v mene používateľov pomocou prostredia PowerShell**. Nemôže odvolať správy z admin center.
- Môžete **len recall správy, ktoré odosielajú ľudí vo vašej organizácii**. Ak bola odoslaná na adresu služby Gmail, napríklad, nemôžem spomenúť to.
- Môžete **len recall správy odoslané z programu Outlook 2016 v počítači**. Ak používateľ odošle správu pomocou programu Outlook for Mac alebo Outlook na webe, si nemôžete spomenúť.

Ak chcete odvolať alebo nahradiť e-mailovej správy:

1. Na table priečinkov v ľavej časti okna programu Outlook vyberte priečinok Sent Items.
1. Správu chcete odvolať ho otvorte dvojitým kliknutím.
1. Vyberte **správy** kartu, a potom vyberte **akcie** > **Odvolanie tejto správy**.
1. Vyberte **Odstrániť neprečítané kópie tejto správy** alebo **Odstrániť neprečítané kópie a nahradiť novú správu**, a potom kliknite na **tlačidlo OK**.
1. Ak posielate správu náhradné, napísať správu a vyberte položku **Odoslať**.
1. Úspech či neúspech odvolanie správy závisí od príjemcu nastavenia v programe Outlook. Kroky na kontrolu, na stiahnutie, nájdete v [tomto článku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Vyhľadanie a odstránenie e-mailových správ v organizácii

- Ak si nie ste globálne admin, váš účet musí pripočítať k eDiscovery Manager úlohu alebo súlad vyhľadávanie rola na vyhľadávanie správ. Ak chcete odstrániť správy, musíte pripojiť sa k skupine rolí Správa organizácie alebo Hľadať a očistenie rola. [Centrum zabezpečenia a súladu](https://go.microsoft.com/fwlink/?linkid=2083731)sú priradené povolenia pre tieto úlohy.
- [Vytvoriť obsah vyhľadávať](https://docs.microsoft.com/office365/securitycompliance/content-search) správy odstrániť.
- [Pripojiť k bezpečnosti a centrum súladu PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ak používate viacerými autentizácia, nájdete [pripojenie k Office 365 zabezpečenia a súladu centrum PowerShell pomocou viacnásobné overovanie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).