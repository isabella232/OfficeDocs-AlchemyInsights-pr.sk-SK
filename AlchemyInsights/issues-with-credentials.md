---
title: Problémy s povereniami
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063687"
---
# <a name="issues-with-credentials"></a>Problémy s povereniami

[Platforma Microsoft identity a tok poverení klienta oauth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) popisujú, ako program priamo v porovnaní s povereniami klienta OAuth 2,0 udeliť tok.

**Ako môžem spravovať poverenia na zadanie hesla alebo certifikátu aplikácie?**

V platforme Azure CLI môžete na odstránenie, zoznam alebo vynulovanie poverení hesla alebo certifikátu aplikácie použiť [poverenia služby AZ ad](https://docs.microsoft.com/cli/azure/ad/app/credential) .

**Ako si používatelia vynulujú svoje heslá?**

Používatelia sa musia [zaregistrovať na samoobslužné vytvorenie nového hesla](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) predtým, ako budú môcť obnoviť svoje heslá. Keď sa používateľ zaregistroval, môže podľa pokynov v tomto článku vytvoriť nové heslo: [Vytvorenie nového pracovného alebo školského hesla](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Ako používatelia zmenia svoje heslá?**

Používatelia môžu postupovať podľa krokov v tomto článku na zmenu hesla: [ako zmeniť heslo](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Môžu tiež [Spravovať heslá aplikácií pre dvojstupňové overovanie](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Používateľovi sa zobrazuje chyba pri zmene alebo resetovaní hesla**

Toto prepojenie poskytne informácie o bežných problémoch, ktoré sa môžu vyskytnúť pri pokuse používateľa o vytvorenie nového hesla: [bežné problémy a ich riešenia](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Mám problém s obnovením hesla používateľa**

- Uistite sa, že máte oprávnenie na vytvorenie nového hesla. *Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov.* Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.

- Uistite sa, že chápete licenčné požiadavky:

  - V organizácii musíte mať priradenú aspoň jednu licenciu:
    - **Iba používatelia cloudu** – všetky platené jednotky SKU služieb Office 365 (O365) alebo Azure AD Basic
    - **Cloudové a/alebo lokálne používatelia** – Azure AD Premium P1 alebo P2, Enterprise mobility + Security (EMS) alebo zabezpečený produktívny podnik (SPE)
    - Ďalšie informácie o licenčných požiadavkách nájdete [v téme licenčné požiadavky na vytvorenie nového hesla služby Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Ak chcete vytvoriť nové heslo používateľa, vyhľadajte používateľa v službe Azure AD. Potom v prehľade Blade pre daného používateľa kliknite na tlačidlo vytvoriť nové heslo.

**Tlačidlo na vytvorenie nového hesla je sivé**

Nemáte oprávnenie na vytvorenie nového hesla **tohto** používateľa. *Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov.* Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.

**Nezobrazuje sa vám čepeľ na vytvorenie nového hesla**

Nemáte oprávnenie na vytvorenie nového hesla. *Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov.* Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.

**V časti Vytvorenie nového hesla sa nezobrazuje lokálna integračná čepeľ**

- Lokálna integračná čepeľ sa zobrazuje len v hybridných prostrediach, čo znamená, že používate heslo zápisom na manipuláciu s heslami lokálneho používateľa.

- Táto čepeľ sa nezobrazuje, ak:

  - Nepoužívate heslo zápisom
  - Vyskytol sa problém s inštaláciou alebo pripojením hesla zápisom
  - Vyskytol sa problém s inštaláciou alebo pripojením služby Azure AD Connect
  - Ďalšie kroky na riešenie problémov s heslom zápisom nájdete v téme [Riešenie problémov s heslom zápisom](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Neviem, ako vytvoriť nové heslo používateľa**

1. Prihláste sa na portáli Azure ako príslušný správca.
2. Prejdite na čepeľ **Používatelia a skupiny** , vyberte položku **všetci používatelia**.
3. Vyberte používateľa v zozname.
4. Pre vybratého používateľa vyberte položku **Prehľad** a potom na paneli príkazov vyberte položku **vytvoriť nové heslo**.
5. Vyberte tlačidlo **vynulovať heslo** a postupujte podľa pokynov na obrazovke.
    - Obnoví sa len prostredníctvom zápisom hesla podpory **platformy Azure Portal** .

**Pri resetovaní hesla lokálneho používateľa na portáli pre správcov služieb Office 365 alebo v mobilnej aplikácii balíka Office 365 sa používateľ stále nedokáže prihlásiť**

Na tomto portáli nie je podporovaná zápisom hesla. Znova obnovte heslo používateľa na portáli Azure.
