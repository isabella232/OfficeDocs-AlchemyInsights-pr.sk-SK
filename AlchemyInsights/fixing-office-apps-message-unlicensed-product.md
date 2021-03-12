---
title: Office sa nedá aktivovať
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704945"
---
# <a name="unable-to-activate-office"></a>Office sa nedá aktivovať

- Skontrolujte, či vám neuplynula platnosť predplatného.
- Uistite sa, že máte predplatné, ktoré umožňuje klientske licencie ako Office 365 Business alebo Business Premium a [uistite sa, že používateľ má priradenú licenciu](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).
- Uistite sa, že používateľ sa prihlasuje do balíka Office s kontom, ktoré má priradenú licenciu.
- Na [stránke Stav služby Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) skontrolujte, či sa nevyskytujú známe problémy so službou.
- Skontrolujte nastavenia brány firewall, antivírusového softvéru a nastavení servera proxy a potvrďte, že neblokujú aplikáciám Microsoftu 365 prístup na internet. Pozrite si tému [URL adresy a rozsahy IP adries v balíku Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL adresy a rozsahy IP adries služieb Office 365").

**Tip** Na zariadeniach s Windowsom pre vás môžeme diagnostikovať a automaticky opraviť niekoľko bežných problémov s prihlasovaním na do balíka Office. Stiahnite a spustite asistenta **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)**, aby ste mohli používať náš automatický nástroj.

Postupujte podľa týchto krokov na riešenie problémov:

- Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) zo všetkých existujúcich používateľských kont. [Odstráňte](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) a [znova priraďte](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licenciu na Office a potom [sa prihláste do balíka Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocou ovplyvneného používateľského konta.
- Spustite nástroj [Poradca pri riešení problémov s aktiváciou](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Obnovte stav aktivácie balíka Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Obnovte stav aktivácie balíka Office")
- [Vykonanie online opravy balíka Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Ďalšie riešenie problémov nájdete v téme:  

- [Chyba produktu bez platnej licencie a chyba aktivácie v Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Chyba „Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr“ pri aktivácii balíka Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)