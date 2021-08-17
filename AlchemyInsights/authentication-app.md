---
title: Aplikácia na overovanie
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082957"
---
# <a name="authentication-app"></a>Aplikácia na overovanie

Ak ste globálny správca, pomocou diagnostických nástrojov na prihlásenie môžete rýchlo zistiť, čo sa stalo, alebo diagnostikovať problémy súvisiace s [prihlásením používateľov.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Spustite diagnostiku kliknutím na tlačidlo[Spustiť diagnostiku.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Udalosť, ktorú chcete analyzovať, nájdete zadaním podrobností o používateľovi, aplikácii, čase prihlásenia, identifikácii požiadavky alebo identifikácii korelácie.
1. Skontrolujte diagnostické výsledky a pozrite si podrobnosti o tom, čo sa udialo, a aké akcie môžete vykonať na jej zmenu v prípade potreby.

**Skontrolujte scenár, ktorý je k dispozícii:**

1. Ak sa používateľovi v aplikácii na overenie Microsoft Authenticator nezobrazuje oznámenie, ako je to popísané v časti Blokovanie a odblokovanie používateľov, overte, či sa v mfa [blokovaných používateľoch nezobrazuje.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Ak používateľ nie je zablokovaný pre MFA, ale nedoručil oznámenie, môže otvoriť aplikáciu Microsoft Authenticator, ktorá vytiahne čakajúce žiadosti o schválenie.
1. Ako alternatívny spôsob prihlásenia môže používateľ kliknúť aj na položku Prihlásiť sa iným spôsobom a vybrať si z mojej mobilnej aplikácie overovací kód.
1. Aplikácia Microsoft Authenticator je jediným dostupným spôsobom pre mnohých používateľov. [Ďalšie informácie o predvolených nastaveniach](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)zabezpečenia nájdete [v Authenticator Najčastejšie](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) otázky o aplikácii a ich riešení.
 
**Odporúčané videá**

[Ako nastaviť aplikáciu Authenticator v novom telefóne (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
