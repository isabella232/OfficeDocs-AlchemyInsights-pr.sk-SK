---
title: Office sa nedá aktivovať
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798695"
---
# <a name="unable-to-activate-office"></a>Office sa nedá aktivovať

**Poznámka:** Ak používate staršiu verziu balíka Windows (napríklad Windows 7), uistite sa, že protokol TLS 1.2 je predvolene povolený. Ďalšie informácie nájdete v téme Aktualizácia na povolenie [tls 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)ako predvolených zabezpečených protokolov vo WinHTTP v Windows.

- Skontrolujte, či vám neuplynula platnosť predplatného.
- Uistite sa, že máte predplatné, ktoré umožňuje klientske licencie ako Office 365 Business alebo Business Premium a [uistite sa, že používateľ má priradenú licenciu](/microsoft-365/admin/manage/assign-licenses-to-users).
- Uistite sa, že používateľ sa prihlasuje do balíka Office s kontom, ktoré má priradenú licenciu.
- Na [stránke Stav služby Office 365](/office365/enterprise/view-service-health) skontrolujte, či sa nevyskytujú známe problémy so službou.
- Skontrolujte nastavenia brány firewall, antivírusového softvéru a nastavení servera proxy a potvrďte, že neblokujú aplikáciám Microsoftu 365 prístup na internet. Pozrite si tému [URL adresy a rozsahy IP adries v balíku Office 365](/office365/enterprise/urls-and-ip-address-ranges "URL adresy a rozsahy IP adries služieb Office 365").

**Tip** Na zariadeniach s Windowsom pre vás môžeme diagnostikovať a automaticky opraviť niekoľko bežných problémov s prihlasovaním na do balíka Office. Stiahnite a spustite asistenta **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)**, aby ste mohli používať náš automatický nástroj.

Postupujte podľa týchto krokov na riešenie problémov:

- Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) zo všetkých existujúcich používateľských kont. [Odstráňte](/microsoft-365/admin/manage/remove-licenses-from-users) a [znova priraďte](/microsoft-365/admin/manage/assign-licenses-to-users) licenciu na Office a potom [sa prihláste do balíka Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocou ovplyvneného používateľského konta.
- Spustite nástroj [Poradca pri riešení problémov s aktiváciou](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Obnovte stav aktivácie balíka Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Obnovte stav aktivácie balíka Office")
- [Vykonanie online opravy balíka Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Ďalšie riešenie problémov nájdete v téme:  

- [Chyba produktu bez platnej licencie a chyba aktivácie v Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Chyba „Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr“ pri aktivácii balíka Office](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)