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
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430215"
---
# <a name="troubleshoot-sspr"></a>Riešenie problémov s SSPR

**Mám problémy s konfiguráciou nového hesla**

- Ak ste správcom a hľadáte spôsob, ako povoliť samoobslužné vytvorenie nového hesla, pozrite si tému [povolenie SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)na konfigurovanie obnovenia nového hesla pre vašu organizáciu. Môžete tiež skontrolovať [licenčné požiadavky](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). V organizácii musíte mať priradenú aspoň jednu licenciu.
    - **Iba používatelia cloudu** – všetky platené jednotky SKU služieb Office 365 (O365) alebo Azure AD Basic
    - **Cloudové a/alebo lokálne používatelia** – Azure AD Premium P1 alebo P2, Enterprise mobility + Security (EMS) alebo zabezpečený produktívny podnik (SPE)
- Ďalšie otázky o automatickom resetovaní hesla nájdete v [téme Najčastejšie otázky](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Zobrazuje sa chybové hlásenie**

V tomto článku nájdete informácie o bežných chybách a ich riešeniach: [Riešenie problémov s vlastným servisným vynulovaním hesla](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mám problém s politikou na vytvorenie nového hesla**

- Ak sa politika obnovenia hesla nespráva podľa očakávaní alebo ak máte otázky týkajúce sa politík na vytvorenie nového hesla, prečítajte si tento článok: [politiky a obmedzenia hesiel v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Politiky na vytvorenie nového hesla sa nevzťahujú na správcov. Spoločnosť Microsoft vynúti silnú predvolenú politiku na vytvorenie nového hesla s dvoma bránami pre ľubovoľnú rolu správcu služby Azure. Uistite sa, že skúšate používateľa, ktorý nie je správcom. Ďalšie informácie o politike obnovenia správcu nájdete v téme tento článok: [Obnovenie zásad politiky správcu](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Nechcem, aby moji používatelia zaregistrovali ďalšie bezpečnostné informácie na vytvorenie nového hesla**

Pre používateľov môžete vopred vyplniť údaje (e-maily a telefónne atribúty) pomocou rozhrania API, PowerShell alebo služby Azure AD Connect. Ak sa chcete dozvedieť, ako čítať:

- [Nasadenie nového hesla bez nutnosti registrácie používateľov](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Aké údaje sa používajú na vytvorenie nového hesla](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Chcem, aby moji používatelia zaregistrovali ďalšie bezpečnostné informácie na vytvorenie nového hesla**

1. Požiadajte svojich používateľov, aby si zaregistrovali svoje bezpečnostné informácie na vytvorenie nového hesla a nasmerujú ich na [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Po vyplnení údajov používateľovi (používateľom alebo správcom) nasmerujte používateľa na [aka.MS/SSPR](https://passwordreset.microsoftonline.com/) , aby mohli vaši používatelia mať právo na vytvorenie nového hesla.
1. Ak sa stále vyskytujú problémy, ktoré sú s najväčšou pravdepodobnosťou **externý** alebo **hash hesla synchronizovaní** používatelia. To znamená, že je pravdepodobné, že sa vyskytol problém so službou Password zápisom.