---
title: Problém s obnovením hesla
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
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696277"
---
# <a name="problems-resetting-password"></a>Problémy s obnovením hesla

Nižšie sú uvedené niektoré problémy, s ktorými sa môžete stretnúť pri resetovaní hesla a možných riešeniach:

**Mám problém s vytvorením nového hesla, ktoré nie je zahrnuté v iných kategóriách**

- Uistite sa, že máte oprávnenie na vytvorenie nového hesla. Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov. Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.
- Uistite sa, že chápete licenčné požiadavky:
    - V organizácii musíte mať priradenú aspoň jednu licenciu.
        - Iba používatelia cloudu – všetky platené jednotky SKU služieb Office 365 (O365) alebo Azure AD Basic
        - Cloudové a/alebo lokálne používatelia – Azure AD Premium P1 alebo P2, Enterprise mobility + Security (EMS) alebo zabezpečený produktívny podnik (SPE)
        - Ďalšie informácie o licenčných požiadavkách nájdete v článku [licenčné požiadavky na vytvorenie nového hesla služby Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Mám problémy s testovaním politiky na vytvorenie nového hesla**

- Naposledy aplikované politiky môžu trvať niekoľko minút, kým sa replikujú vo všetkých dátových centrách a na koncových bodoch. Fyzická vzdialenosť od dátového centra ovplyvní aj spôsob používania rýchlych zmien.
- Otestujte sa koncovým používateľom, nie správcom, a pilot s malou skupinou používateľov. Politiky nakonfigurované na portáli Azure sa uplatňujú len na koncových používateľov, nie správcov. Spoločnosť Microsoft vynúti silnú predvolenú politiku na vytvorenie nového hesla s dvoma bránami pre ľubovoľnú rolu správcu služby Azure (príklad: globálny správca, správca helpdesk, správca hesiel atď.)
    - Ďalšie informácie o [politikách pre správcov](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Chcem nasadiť vytvorenie nového hesla, ale nechcem, aby moji používatelia zaregistrovali ďalšie bezpečnostné informácie**

Pred vyplnením údajov pre používateľov tak, aby nemuseli. -Ako správca môžete nastaviť vlastnosti telefónu a e-mailu pre svojich používateľov pred vykonaním obnovenia nového hesla vo vašej organizácii. Môžete to urobiť pomocou rozhrania API, PowerShell alebo Azure AD Connect. Ďalšie informácie nájdete tu:
- [Nasadenie nového hesla bez nutnosti registrácie používateľov](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Aké údaje sa používajú na vytvorenie nového hesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Tlačidlo na vytvorenie nového hesla je sivé**

Nemáte oprávnenie na vytvorenie nového hesla tohto používateľa. Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov. Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.

**Nezobrazuje sa vám čepeľ na vytvorenie nového hesla**

Nemáte oprávnenie na vytvorenie nového hesla. Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov. Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.

**V časti Vytvorenie nového hesla sa nezobrazuje lokálna integračná čepeľ**

- Lokálna integračná čepeľ sa zobrazuje len v hybridných prostrediach, čo znamená, že používate heslo zápisom na manipuláciu s heslami lokálneho používateľa.
- Táto čepeľ sa nezobrazuje, ak:
    - Nepoužívate heslo zápisom
    - Vyskytol sa problém s inštaláciou alebo pripojením hesla zápisom
    - Vyskytol sa problém s inštaláciou alebo pripojením služby Azure AD Connect
    - Ďalšie kroky na riešenie problémov s heslom zápisom nájdete v časti [Riešenie problémov s heslom zápisom](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Neviem, ako vytvoriť nové heslo používateľa**

1. Prihláste sa na portáli Azure ako príslušný správca.
1. Prejdite na čepeľ používatelia a skupiny, vyberte položku **všetci používatelia**.
1. Vyberte používateľa v zozname.
1. Pre vybratého používateľa vyberte položku **Prehľad** a potom na paneli príkazov kliknite na položku **vytvoriť nové heslo**.
1. Postupujte podľa pokynov na obrazovke.
    - Obnoví sa len prostredníctvom zápisom hesla podpory platformy Azure Portal.

**Pri resetovaní hesla lokálneho používateľa na portáli pre správcov služieb Office 365 alebo v mobilnej aplikácii balíka Office 365 sa používateľ stále nedokáže prihlásiť**

Na tomto portáli nie je podporovaná zápisom hesla. Opätovné vytvorenie nového hesla používateľa na portáli Azure – portal.azure.com

