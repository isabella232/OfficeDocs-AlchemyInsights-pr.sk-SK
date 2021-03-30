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
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405680"
---
# <a name="authentication-app"></a>Aplikácia na overovanie

Ak ste globálny správca, pomocou diagnostických nástrojov na prihlásenie môžete rýchlo zistiť, čo sa stalo, alebo diagnostikovať problémy súvisiace s [prihlásením používateľov.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Spustite diagnostiku kliknutím na tlačidlo[Spustiť diagnostiku.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Udalosť, ktorú chcete analyzovať, nájdete zadaním podrobností o používateľovi, aplikácii, čase prihlásenia, identifikácii požiadavky alebo identifikácii korelácie.
1. Skontrolujte diagnostické výsledky a pozrite si podrobnosti o tom, čo sa udialo, a aké akcie môžete vykonať na jej zmenu v prípade potreby.

**Skontrolujte scenár, ktorý je k dispozícii:**

1. Ak sa používateľovi v aplikácii Microsoft Authenticator nezobrazuje oznámenie bez oznámenia, overte, či sa nezobrazuje v časti Zablokovaní používatelia mfa, ako je to popísané v časti Blokovanie a [odblokovanie používateľov.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Ak používateľ nie je zablokovaný pre MFA, ale nedoručuje sa upozornenie, môže otvoriť aplikáciu Microsoft Authenticator, ktorá vytiahne čakajúce žiadosti o schválenie.
1. Ako alternatívny spôsob prihlásenia môže používateľ kliknúť aj na položku Prihlásiť sa iným spôsobom a vybrať si z mojej mobilnej aplikácie overovací kód.
1. Aplikácia Microsoft Authenticator je jediným dostupným spôsobom pre mnohých používateľov. [Prečítajte si ďalšie informácie o predvolených nastaveniach](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)zabezpečenia, najčastejšie [otázky o aplikácii Authenticator a](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) zistite, ako ich vyriešiť.
 
**Odporúčané videá**

[Ako nastaviť aplikáciu Authenticator v novom telefóne (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
