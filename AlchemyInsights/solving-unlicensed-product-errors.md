---
title: Riešenie chýb nelicencovaných produktov
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: 87a0a2be6b222d35acbc862eed4f14fb3e3e36ac
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764168"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Návrhy na riešenie chýb "nelicencovaných produktov"

Ak chcete vyriešiť chyby týkajúce sa "nelicencovaného produktu", vyskúšajte nasledujúce kroky:

- Skontrolujte, či stav predplatného vypršal.
- Uistite sa, že máte predplatné, ktoré umožňuje klientske licencie, napríklad Microsoft 365 aplikácie Business alebo Business Premium a [zabezpečiť, že používateľ má priradenú licenciu](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users). 
- Uistite sa, že používateľ sa prihlasuje do balíka Office s rovnakým kontom, ktoré má priradenú licenciu.
- Skontrolujte [stav služby stránky](https://docs.microsoft.com/office365/enterprise/view-service-health) a zistite, či existujú nejaké známe problémy so službou.
- Skontrolujte, či brána firewall, antivírusový softvér a nastavenia servera proxy potvrdia, že neblokujú prístup aplikácií balíka Office na internet. Pozrite si [adresy URL a rozsahy adries IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Môžete tiež vyskúšať nasledujúce akcie riešenia problémov: 

- Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z existujúcich používateľských kont. [Odstráňte](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users) a [znova priraďte](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) licenciu balíka Office a potom [sa prihláste do balíka Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocou príslušného používateľského konta.
- Spustite [poradcu pri riešení problémov s aktiváciou](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Obnoviť stav aktivácie balíka Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Vykonajte online opravu balíka Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Ďalšie riešenie problémov nájdete v téme: 

- [Chyba produktu bez platnej licencie a chyba aktivácie v Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [Chyba „Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr“ pri aktivácii balíka Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)