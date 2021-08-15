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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986834"
---
# <a name="issues-with-credentials"></a>Problémy s povereniami

Microsoft identity platform poverenia klienta [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) popisujú, ako programovať priamo voči povereniam klienta OAuth 2.0 udeliť tok.

**Ako môžem spravovať heslo aplikácie alebo poverenia certifikátu?**

V Azure CLI môžete použiť poverenia [az ad app](https://docs.microsoft.com/cli/azure/ad/app/credential) na odstránenie, vytvorenie zoznamu alebo vytvorenie nového hesla alebo poverení certifikátu aplikácie.

**Ako môžu používatelia obnovovať heslá?**

Používatelia si pred [obnovením hesiel budú musieť zaregistrovať](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) samoobslužné vytvorenie nového hesla. Po registrácii môže používateľ postupovať podľa pokynov v tomto článku a vytvoriť si nové heslo: Vytvorenie nového [pracovného alebo školského hesla.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Ako môžu používatelia meniť heslá?**

Používatelia môžu zmeniť svoje heslá podľa krokov uvedených v tomto článku: [Zmena hesla.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Môžu tiež spravovať [heslá aplikácií pre dvojstupňové overenie.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Používateľovi sa pri zmene alebo obnovení hesla zobrazuje chyba**

Toto prepojenie poskytne informácie o bežných problémoch, ktoré môžu vzniknúť, keď sa používateľ pokúša vytvoriť nové heslo: bežné problémy a [ich riešenia](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Mám problém s obnovením hesla používateľa**

- Skontrolujte, či máte oprávnenie na vytvorenie nového hesla. *Nové heslá používateľov môžu vytvoriť iba globálni správcovia, heslá používateľov a správcovia používateľov.* Globálni správcovia môžu tiež obnoviť heslá iných privilegovaných správcov.

- Uistite sa, že rozumiete licenčným požiadavkám:

  - Musíte mať vo svojej organizácii priradenú aspoň jednu licenciu:
    - **Len používatelia v cloude** – všetky Office 365 (O365) platené SKU alebo Azure AD Basic
    - **Cloud a/alebo** lokálni používatelia – Azure AD Premium P1 alebo P2, Enterprise Mobility + Security (EMS) alebo Secure Productive Enterprise (SPE)
    - Ďalšie informácie o licenčných požiadavkách nájdete v téme [Licenčné požiadavky na samoobslužné vytvorenie nového hesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)pre Azure AD.
- Ak chcete vytvoriť nové heslo používateľa, vyhľadajte používateľa v službe Azure AD. Potom na prehľade blade pre tohto používateľa kliknite na tlačidlo "vytvoriť nové heslo".

**Tlačidlo na vytvorenie nového hesla je sivé**

Nemáte oprávnenie resetovať **heslá** tohto používateľa. *Nové heslá používateľov môžu vytvoriť iba globálni správcovia, heslá používateľov a správcovia používateľov.* Globálni správcovia môžu tiež obnoviť heslá iných privilegovaných správcov.

**Nevidím blade na vytvorenie nového hesla**

Nemáte oprávnenie na vytvorenie nového hesla. *Nové heslá používateľov môžu vytvoriť iba globálni správcovia, heslá používateľov a správcovia používateľov.* Globálni správcovia môžu tiež obnoviť heslá iných privilegovaných správcov.

**Lokálnu serveri integrácie sa v obnovení hesiel nevidím**

- Server blade s lokálnou integráciou sa zobrazuje len v hybridných prostrediach, čo znamená, že na manipuláciu s heslami lokálnych používateľov používate spätné písanie hesla.

- Tento blade sa v tomto prípade:

  - Nepoužívate password writeback
  - Vyskytol sa problém s inštaláciou/pripojiteľnosťou funkcie writeback hesla
  - Vyskytol sa problém s inštaláciou/pripojením služby Azure AD Pripojenie
  - Ďalšie kroky na riešenie problémov s písaním hesla nájdete v téme Riešenie problémov [s heslom na spätné písanie](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Neviem, ako vytvoriť nové heslo používateľa**

1. Prihláste sa na portál Azure ako vhodný správca.
2. Prejdite na blade **Users and groups (Používatelia a** skupiny), vyberte položku All Users **(Všetci používatelia).**
3. V zozname vyberte používateľa.
4. Pre vybratého používateľa vyberte položku **Prehľad** a potom na paneli príkazov vyberte položku **Vytvoriť nové heslo**.
5. Vyberte tlačidlo **Vytvoriť nové** heslo a postupujte podľa pokynov na obrazovke.
    - Obnovenie vykonané prostredníctvom portálu **Azure podporuje iba** spätné písanie hesla.

**Obnovenie hesla lokálneho používateľa z portálu Office 365 Admin alebo mobilnej aplikácie Office 365 používateľ sa však stále nemôže prihlásiť**

Na tomto portáli nie je podporovaná ochrana heslom. Na portáli Azure znova obnovte heslo používateľa.
