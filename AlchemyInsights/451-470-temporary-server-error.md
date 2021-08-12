---
title: 451 4.7.0 Dočasná chyba servera. Skúste to znova neskôr. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812590"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Dočasná chyba servera. Skúste to znova neskôr. PRX4

Pri odosielaní e-mailu prostredníctvom služby Smarthost smtp.office365.com sa môže zobraziť problém pomocou metódy odosielania klienta SMTP a zobrazí sa chyba: "451 4.7.0 Dočasná chyba servera. Skúste to znova neskôr. PRX4 je väčšinou dočasný." 

Skontrolujte, či nepoužívate zdieľanú poštovú schránku na odosielanie klienta SMTP, pretože metóda odosielania klienta SMTP vyžaduje na odoslanie pošty licencovanú poštovú schránku. Ak však nepoužívate zdieľanú poštovú schránku a problém pretrváva, skontrolujte toto:

1. Povoľte odosielanie protokolu SMTP klienta v licencovanej poštovej schránke, ktorá sa používa spustením tohto príkazu prostredia PowerShell:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    ALEBO

    1. Prejdite na Centrum spravovania služby Microsoft 365 > **Aktívni používatelia** a vyberte používateľa.
    1. Prejdite na kartu Pošta a > **aplikácie e->** položku **Spravovať e-mailové aplikácie**. 
    1. Skontrolujte, či je začiarknuté (zapnuté) nastavenie Overený **SMTP.**
    1. Vyberte **položku Save changes (Uložiť zmeny).**
    
    Ak chcete zapnúť overenie SMTP pre celú organizáciu, spustite tento príkaz:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Poznámka:** Z bezpečnostných dôvodov sa odporúča zapnúť overenie SMTP iba pre používanú poštovú schránku. Nastavenie na úrovni používateľa prepíše nastavenie úrovne organizácie.

2. Vypnite predvolené nastavenia zabezpečenia služby Azure pre vypnutie možnosti **Povoliť predvolené nastavenia zabezpečenia** na možnosť **Nie:**

    1. Prihláste sa na portál Azure ako správca zabezpečenia, ako správca podmieneného prístupu alebo globálny správca.
    1. Vyhľadajte položku Azure Active Directory >**  a** vyberte položku **Správa predvolených nastavení zabezpečenia**.
    1. Nastavte **prepínač Povoliť predvolené nastavenia** zabezpečenia na možnosť **Nie.**
    1. Vyberte **položku Uložiť**.

3. Vypnite viacfaktorové overovanie (MFA) v poštovej schránke s licenciou, ktorá sa používa.

    1. Prejdite na navigačnú Centrum spravovania služby Microsoft 365 a v ľavej navigačnej ponuke vyberte položku **Používatelia**  >  **Aktívni používatelia.**
    1. Na stránke **Aktívni** používatelia vyberte položku **Viacfaktorové overovanie**.
    1. Vyberte používateľa a vypnite **viacfaktorové overovanie.**

