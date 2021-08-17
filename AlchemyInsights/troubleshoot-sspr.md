---
title: Riešenie problémov s SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038973"
---
# <a name="troubleshoot-sspr"></a>Riešenie problémov s SSPR

**Mám problém s konfiguráciou vynulovania hesiel**

- Ak ste správcom a hľadáte postup, ako zapnúť samoobslužné vytvorenie nového hesla, pozrite si kurz povolenia [SSPR,](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)kde môžete nakonfigurovať vytvorenie nového hesla pre svoju organizáciu. Môžete si tiež skontrolovať [licenčné požiadavky](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Musíte mať vo svojej organizácii priradenú aspoň jednu licenciu.
    - **Len používatelia v cloude** – všetky Office 365 (O365) platené SKU alebo Azure AD Basic
    - **Cloud a/alebo** lokálni používatelia – Azure AD Premium P1 alebo P2, Enterprise Mobility + Security (EMS) alebo Secure Productive Enterprise (SPE)
- Ďalšie otázky týkajúce sa samoobslužných vytvorenie nového hesla nájdete v [našich najčastejších otázkach.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zobrazuje sa chybové hlásenie**

V tomto článku nájdete bežné chyby a ich riešenia: Riešenie problémov s [samoobslužne vytvorenie nového hesla](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mám problém s moju politiku na vytvorenie nového hesla**

- Ak sa politika na vytvorenie nového hesla nespráva podľa očakávania alebo ak máte otázky týkajúce sa politík obnovenia hesiel, pozrite si tento článok: Politiky a obmedzenia [hesiel vo Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Politiky pri obnove hesiel sa nevzťahujú na správcov. Spoločnosť Microsoft vynucuje silné predvolené politiky pri obnove hesiel dvoch brán pre všetky roly správcu Azure. Skontrolujte, či testujete s používateľom, ktorý nie je správcom. Ďalšie informácie o politike obnovenia výrobných nastavení nájdete v tomto článku: Rozdiely v politike [pri obnove zo správcov.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Nechcem, aby používatelia registrovali ďalšie bezpečnostné informácie na vytvorenie nového hesla**

Údaje (atribúty e-mailu a telefónu) môžete vopred vyplniť pomocou rozhrania API, prostredia PowerShell alebo služby Azure AD Pripojenie. Ak chcete zistiť, ako čítať:

- [Nasadenie nového hesla bez nutnosti registrácie používateľov](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Aké údaje sa používajú pri obnovení hesiel](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Chcem, aby používatelia zaregistrovali svoje dodatočné bezpečnostné informácie na vytvorenie nového hesla**

1. Nasmerujte používateľov, aby si zaregistrovali svoje bezpečnostné informácie na samoobslužné vytvorenie nového hesla tak, že ich [nasmerujú aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Po vyplnení údajov používateľa (používateľom alebo správcom) nasmerujte používateľa [na aka.ms/sspr,](https://passwordreset.microsoftonline.com/) aby si používatelia mohli aj sami vytvoriť nové heslá.
1. Ak sa u používateľov stále  vyskytujú problémy, pravdepodobne majú synchronizovaný federovaný používatelia alebo **synchronizovaný používatelia s hash hesiel.** To znamená, že pravdepodobne sa vyskytol problém so službu Password Writeback.