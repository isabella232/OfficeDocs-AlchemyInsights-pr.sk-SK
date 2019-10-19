---
title: Outlook Desktop Recall alebo nahradiť e-mailovú správu
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36496126"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Vyvolanie alebo nahradenie e-mailovej správy programu Outlook

- Ako admin, môžete **pripomenúť správy v mene používateľov pomocou PowerShell**. Správy z centra spravovania nemožno vyvolať.
- Môžete **pripomenúť iba správy odoslané ľuďom vo vašej organizácii**. Ak bola správa odoslaná na adresu služby Gmail, nemôžete ju napríklad pripomenúť.
- Môžete si **len pripomenúť správy odoslané z programu Outlook 2016 na PC**. Ak používateľ odošle správu pomocou programu Outlook for Mac alebo Outlook na webe, nemôžete pripomenúť.

Ak chcete pripomenúť alebo nahradiť e-mailovú správu:

1. Na table priečinkov v ľavej časti okna programu Outlook vyberte priečinok Odoslaná pošta.
1. Dvakrát kliknite na správu, ktorú chcete pripomenúť, aby ste ju otvorili.
1. Vyberte kartu **Správa** a potom vyberte **akcie** > **vyvolanie tejto správy**.
1. Vyberte položku **Odstrániť neprečítané kópie tejto správy** alebo **odstráňte neprečítané kópie a nahraďte ju novou správou**a potom kliknite na **tlačidlo OK**.
1. Ak odosielate náhradnú správu, Vytvorte správu a potom vyberte položku **Odoslať**.
1. Úspech alebo neúspech odvolanie správy závisí od nastavenia príjemcu v programe Outlook. Postup na kontrolu stiahnutia z trhu nájdete [v tomto článku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Vyhľadávanie a odstraňovanie e-mailových správ vo vašej organizácii

- Ak nie ste globálny správca, konto sa musí pridať do roly správcu eDiscovery alebo roly správy vyhľadávania súladu, aby ste mohli vyhľadávať správy. Ak chcete odstrániť správy, musíte sa pripojiť k skupine rolí Správa organizácie alebo k úlohe správy vyhľadávania a čistenia. Povolenia pre tieto roly sú priradené v [Centre zabezpečenia a súladu](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Vytvorte hľadanie obsahu](https://docs.microsoft.com/office365/securitycompliance/content-search) a vyhľadajte správu, ktorá sa má odstrániť.
- [Pripojiť k zabezpečenia a súladu centrum PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ak používate viacnásobné overovanie, pozrite si [pripojenie k Office 365 zabezpečenia a súladu centrum PowerShell pomocou viacnásobné overovanie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).