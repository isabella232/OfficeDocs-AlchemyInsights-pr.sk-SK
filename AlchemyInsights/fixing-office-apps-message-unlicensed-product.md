---
title: Balík Office sa nedá aktivovať
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: ee4618bd288e3e8be75dc969af58f921a14f48b0
ms.sourcegitcommit: bf87d91fa60bd961bc6c887c4a4be7a3c7665b38
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/01/2020
ms.locfileid: "44474512"
---
# <a name="unable-to-activate-office"></a>Balík Office sa nedá aktivovať

- Skontrolujte, či vám neuplynula platnosť predplatného.
- Uistite sa, že máte predplatné, ktoré umožňuje klientske licencie, napríklad Office 365 Business alebo Business Premium, a [uistite sa, že používateľ má priradenú licenciu](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).
- Uistite sa, že používateľ sa prihlasuje do balíka Office s tým istým kontom, ktoré má priradenú licenciu.
- Na [stránke Stav služby Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) skontrolujte, či sa nevyskytujú známe problémy so službou.
- Skontrolujte nastavenia brány firewall, antivírusového softvéru a nastavení servera proxy a potvrďte, že neblokujú aplikáciám balíka Office prístup na internet. Pozrite si tému [URL adresy a rozsahy IP adries v balíku Office 365](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges "URL adresy a rozsahy IP adries v Office 365").

Postupujte podľa týchto krokov na riešenie problémov:

- Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) zo všetkých existujúcich používateľských kont. [Odstráňte](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users?view=o365-worldwide "Odstrániť") a [znova priraďte](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide "znova priradiť") licenciu na Office a potom [sa prihláste do balíka Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "prihlásenie do balíka Office") pomocou ovplyvneného používateľského konta.
- Spustite nástroj [Poradca pri riešení problémov s aktiváciou](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Obnovte stav aktivácie balíka Office](https://docs.microsoft.com/en-us/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Obnovenie stavu aktivácie balíka Office")
- [Vykonanie online opravy balíka Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Ďalšie riešenie problémov nájdete v téme:  
[Chyba produktu bez platnej licencie a chyba aktivácie v Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)  
["Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr" chyba pri aktivácii balíka Office]( https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365 "Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr" chyba pri aktivácii balíka Office")