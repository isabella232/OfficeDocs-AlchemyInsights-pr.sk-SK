---
title: Problém s vytvorením nového hesla
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039981"
---
# <a name="problems-resetting-password"></a>Problémy s obnovením hesla

Nižšie sú uvedené niektoré problémy, s ktoré sa môžete čudovať pri obnovení hesla a možné riešenia:

**Mám problém s obnovením hesla, ktoré sa nezaosiela v ostatných kategóriách**

- Uistite sa, že máte oprávnenie na vytvorenie nového hesla. Nové heslá používateľov môžu vytvoriť iba globálni správcovia, heslá používateľov a správcovia používateľov. Globálni správcovia môžu tiež obnoviť heslá iných privilegovaných správcov.
- Uistite sa, že rozumiete licenčným požiadavkám:
    - Musíte mať vo svojej organizácii priradenú aspoň jednu licenciu
        - Len používatelia v cloude – Office 365 (O365) platené SKU alebo Azure AD Basic
        - Cloud a/alebo lokálni používatelia – Azure AD Premium P1 alebo P2, Enterprise Mobility + Security (EMS) alebo Secure Productive Enterprise (SPE)
        - Ďalšie informácie o licenčných požiadavkách nájdete v článku Licenčné [požiadavky na samoobslužné](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)vytvorenie nového hesla pre Azure AD.

**Mám problémy s testovaním nastavení politiky obnovenia hesiel**

- Nedávno použité politiky môžu trvať niekoľko minút, kým sa replikujú vo všetkých údajových centrách a koncových bodoch. Fyzická vzdialenosť od údajového centra ovplyvní aj to, ako rýchlo sa zmeny použijú.
- Otestujte sa s koncovým používateľom, nie správcom a pilotným používateľom s malou množinou používateľov. Politiky nakonfigurované na portáli Azure sa vzťahujú LEN na koncových používateľov, nie na správcov. Spoločnosť Microsoft vynucuje štandardnú predvolenú politiku obnovenia hesiel pomocou dvoch brán pre všetky roly správcu platformy Azure (Príklad: Globálny správca, Správca technickej podpory, Správca hesiel atď.)
    - Ďalšie informácie o [politikách pre správcov.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Chcem nasadiť vytvorenie nového hesla, ale nechcem, aby používatelia registrovali ďalšie bezpečnostné informácie**

Vopred vyplňte údaje pre používateľov, aby to nebolo potrebné. – Ako správca môžete pre používateľov nastaviť vlastnosti telefónu a e-mailu predtým, ako začnete vo svojej organizácii vytvoriť nové heslo. Môžete to urobiť pomocou rozhrania API, prostredia PowerShell alebo služby Azure AD Pripojenie. Ďalšie informácie nájdete tu:
- [Nasadenie nového hesla bez nutnosti registrácie používateľov](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Aké údaje sa používajú pri obnovení hesiel](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tlačidlo na vytvorenie nového hesla je sivé**

Nemáte oprávnenie resetovať heslá tohto používateľa. Nové heslá používateľov môžu vytvoriť iba globálni správcovia, heslá používateľov a správcovia používateľov. Globálni správcovia môžu tiež obnoviť heslá iných privilegovaných správcov.

**Nevidím blade na vytvorenie nového hesla**

Nemáte oprávnenie na vytvorenie nového hesla. Nové heslá používateľov môžu vytvoriť iba globálni správcovia, heslá používateľov a správcovia používateľov. Globálni správcovia môžu tiež obnoviť heslá iných privilegovaných správcov.

**Lokálnu serveri integrácie sa v obnovení hesiel nevidím**

- Server blade s lokálnou integráciou sa zobrazuje len v hybridných prostrediach, čo znamená, že na manipuláciu s heslami lokálnych používateľov používate spätné písanie hesla.
- Tento blade sa v tomto prípade:
    - Nepoužívate password writeback
    - Vyskytol sa problém s inštaláciou/pripojiteľnosťou funkcie writeback hesla
    - Vyskytol sa problém s inštaláciou/pripojením služby Azure AD Pripojenie
    - Ďalšie kroky na riešenie problémov s písaním hesla nájdete v časti Riešenie problémov s [heslom pomocou funkcie writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Neviem, ako vytvoriť nové heslo používateľa**

1. Prihláste sa na portál Azure ako vhodný správca.
1. Prejdite na blade Users and groups (Používatelia a skupiny), **vyberte položku All Users (Všetci používatelia).**
1. V zozname vyberte používateľa.
1. Pre vybratého používateľa vyberte položku **Prehľad** a potom na paneli príkazov kliknite na položku **Vytvoriť nové heslo**.
1. Postupujte podľa pokynov na obrazovke.
    - Obnovenie vykonané prostredníctvom portálu Azure podporuje iba spätné písanie hesla.

**Obnovenie hesla lokálneho používateľa z portálu Office 365 Admin alebo mobilnej aplikácie Office 365 používateľ sa však stále nemôže prihlásiť**

Na tomto portáli nie je podporovaná ochrana heslom. Obnovte heslo používateľa znova na portáli Azure – portal.azure.com

