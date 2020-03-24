---
title: Bežné problémy so službou Teams pre zákazníkov v oblasti vzdelávania
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 81b80d76530327767bc58adf2e06e5b7ae265f18
ms.sourcegitcommit: 7d787b8c5af223e2711b4c2a2ca55ce2bdc25aea
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2020
ms.locfileid: "42856812"
---
# <a name="teams-common-issues-for-education-customers"></a>Bežné problémy so službou Teams pre zákazníkov v oblasti vzdelávania

**Pre zákazníkov v oblasti vzdelávania**:

Ak potrebujete pomoc pri nasadzovaní služby Teams na podporu vzdialeného vzdelávania, navštívte [centrum FastTrack](https://www.microsoft.com/fasttrack) a odošlite žiadosť. Pozrite si nasledujúce bežné problémy so službou Teams pre zákazníkov v oblasti vzdelávania:

- Zobrazuje sa vám správa „**Prichádzate o to!**“? Nezabudnite [Povoliť službu Microsoft Teams pre vašu školu](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). Pre nájomníkov EDU nie je aplikácia Microsoft Teams predvolene povolená. Musíte ju najprv zapnúť.

- **Ešte ste s aplikáciou Teams nepracovali?** Prečítajte si tému [Výučba a učenie sa na diaľku v Office 365 Education](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4), kde nájdete najnovšie pokyny na nastavenie školy, plánovanie hodín, virtuálne schôdze a zdieľanie obsahu so študentmi.

- Po zapnutí môžu používatelia spúšťať Teams buď inštaláciou [počítačového](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) a [mobilného klienta](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients), alebo z prehliadača na adrese https://teams.microsoft.com.

- **Povolenie hosťovského prístupu pre aplikáciu Teams**: Skontrolujte [kontrolný zoznam hosťovského prístupu do aplikácie Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist) a uistite sa, že boli dokončené všetky kroky.
    - [Informácie o hosťovskom prístupe v aplikácii Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Nastavenie – kontrolný zoznam hosťovského prístupu do aplikácie Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Pripojenie k Team pre hostí](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Schôdze cez Teams a telefonické pripojenie**: Potrebujete pomoc pri zapnutí alebo nastavení audiokonferencií v Microsoft Teams? Bol tento používateľ vytvorený len nedávno? Ak áno, budete musieť počkať 2 až 24 hodín, aby sa nastavenia prejavili. Ak chcete overiť, či používateľ má licenciu na audiokonferencie a má predvolené platené číslo:
    1. Prejdite na položku Aktívni používatelia a potom vyberte príslušného používateľa.
    2. V závislosti od verzie centra spravovania vyberte možnosť **Licencie a aplikácie** alebo kliknite na položku **Upraviť** v okne **Licencie na produkty**.
    3. Skontrolujte, či používateľ má vybraté licencie pre Audiokonferencie, Microsoft Teams a Skype for Business Online (plán 2).
    4. V centre spravovania kliknite na položku **Zobraziť všetko**, potom na položku **Teams**.
    5. V centre spravovania pre Microsoft Teams kliknite na položku **Starší portál**.
    6. V centre spravopvania pre Skype for Business kliknite na položku **Audiokonferencie** a potom **Používatelia**.
    7. Vyberte príslušného používateľa a overte, či má Predvolené platené číslo.

    Ďalšie informácie nájdete v téme [Volacie plány pre Office 365](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) alebo zavolajte tímu Microsoft Commerce Billing, kde vám pomôžu s otázkami týkajúcimi sa licencovania.

    Ďalšie zdroje informácií

    - [Schôdze a konferencie v Microsoft Teams](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Audiokonferencie v Office 365](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Politiky pre schôdze**: Politiky pre schôdze sa používajú na ovládanie funkcií dostupných pre účastníkov schôdzí naplánovaných používateľmi vo vašej organizácii. Po vytvorení politiky a vykonaní zmien môžete politiku priradiť používateľom.

    - **Zmena alebo vytvorenie politiky pre schôdze**: Ak chcete zmeniť alebo vytvoriť politiku schôdze, prejdite na položku **Centrum spravovania pre Microsoft Teams > Schôdze > Politiky pre schôdze**. Vyberte politiku v zozname alebo kliknite na položku **Pridať**. Ak vytvárate novú politiku, pridajte názov a popis. Názov nesmie obsahovať špeciálne znaky a môže mať najviac 64 znakov. Vyberte požadované nastavenia a potom kliknite na tlačidlo **Uložiť**. 
    
        Povedzme napríklad, že máte veľa používateľov a chcete obmedziť šírku pásma, ktorú by ich schôdza vyžadovala. Vytvorili by ste novú vlastnú politiku s názvom Obmedzená šírka pásma a vypnete nasledujúce nastavenia:

        V časti **Zvuk a video**:
        - Vypnite nastavenie **Umožniť nahrávanie cez cloud**.
        - Vypnite nastavenie **Povoliť IP video**.

        V časti **Zdieľanie obsahu**:

        - Zakážte režim zdieľania obrazovky.
        - Vypnite nastavenie **Povoliť tabuľu**.
        - Vypnite nastavenie **Povoliť zdieľané poznámky**.

        Potom **priraďte politiku používateľom**:

    1. V ľavej navigácii centra spravovania pre Microsoft Teams prejdite na položku **Používatelia**, potom kliknite na používateľa.
    2. Vyberte používateľa kliknutím naľavo od mena používateľa a potom kliknite na položku **Upraviť nastavenia**.
    3. V časti **Politika schôdze** vyberte politiku, ktorú chcete priradiť, a potom kliknite na položku **Použiť**.

    Ak chcete politiku priradiť viacerým používateľom naraz, pozrite si tému [Hromadná úprava používateľských nastavení aplikácie Teams](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    Alebo môžete vykonať toto:
    1. V ľavej navigácii centra spravovania pre Microsoft Teams prejdite na položky **Schôdze > Politiky pre schôdze**.
    2. Vyberte politiku kliknutím naľavo od názvu politiku.
    3. Kliknite na položku **Spravovať používateľov**.
    4. Na table **Spravovať používateľov** vyhľadajte používateľa podľa zobrazenovaného mena alebo meno používateľa, vyberte meno a potom kliknite na položku **Pridať**. Zopakujte tento krok pre každého používateľa, ktorého chcete pridať.
    5. Po dokončení pridávania používateľov kliknite na tlačidlo **Uložiť**.

- **Riešenie problému s chýbajúcou klávesnicou na vytáčanie**:
    - Skontrolujte, či má používateľ priradenú [licenciu na Teams](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Skontrolujte, či má používateľ priradený [volací plán](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page).
    - Povoľte pre používateľov funkciu [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Riešenie problémov s prihlásením do aplikácie Teams:** Najprv sa uistite, či je [služba Microsoft Teams v poriadku](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Potom skontrolujte, či sa nevyskytli bežné kódy chýb, a prečítajte si tému [Prečo mám problémy s prihlásením do služby Microsoft Teams?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f) Môžno bude tiež potrebné skontrolovať [modely identity a overovanie v aplikácii Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).
