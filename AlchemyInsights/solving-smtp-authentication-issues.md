---
title: Zapnutie overovania SMTP a riešenie problémov
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
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321768"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Zapnutie overovania SMTP a riešenie problémov

Ak chcete zapnúť overenie SMTP pre poštovú schránku alebo sa vám zobrazuje chyba Klient nie je overený, Overenie neúspešné alebo SmtpClientAuthentication s kódom 5.7.57 alebo 5.7.3 alebo 5.7.139 pri pokuse o prenos e-mailov overením zariadenia alebo aplikácie so systémom Microsoft 365, problém vyriešte vykonaním týchto troch akcií:

1. Ak chcete [vypnúť predvolené nastavenia zabezpečenia služby Azure,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) prepnite možnosť Povoliť predvolené nastavenia zabezpečenia **na** **možnosť Nie.**

    a. Prihláste sa na portál Azure ako správca zabezpečenia, správca podmieneného prístupu alebo globálny správca.<BR/>
    b. Prejdite na Azure Active Directory > **Vlastnosti.**<BR/>
    c. Vyberte **položku Správa predvolených nastavení zabezpečenia.**<BR/>
    d. Možnosť **Povoliť predvolené nastavenia zabezpečenia nastavte** na možnosť **Nie.**<BR/>
    e. Vyberte **položku Uložiť**.

2. [Povoľte odosielanie klientskeho SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) servera v licencovanej poštovej schránke.

    a. V Centrum spravovania služby Microsoft 365 prejdite na **položku Aktívni** používatelia a vyberte používateľa.<BR/>
    b. Prejdite na kartu Pošta a v časti **E-mailové aplikácie vyberte** položku Spravovať **e-mailové aplikácie**.<BR/>
    d. Skontrolujte, **či je začiarknuté políčko** Overený SMTP server (zapnuté).<BR/>
    e. Vyberte **položku Save changes (Uložiť zmeny).**<BR/>

3. [V licencovanej poštovej schránke vypnite](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) viacfaktorové overovanie.

    a. Prejdite na navigačnú Centrum spravovania služby Microsoft 365 a v ľavej navigačnej ponuke vyberte položku **Používatelia**  >  **Aktívni používatelia**.<BR/>
    b. Vyberte **položku Viacfaktorové overovanie.**<BR/>
    c. Vyberte používateľa a vypnite **možnosť Viacfaktorové overovanie.**<BR/>
