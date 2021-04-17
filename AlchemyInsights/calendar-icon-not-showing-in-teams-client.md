---
title: Ikona kalendára sa nezobrazuje v klientovi aplikácie Teams
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
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819968"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Ikona kalendára sa nezobrazuje v klientovi aplikácie Teams

Karta Kalendár v aplikácii Teams vyžaduje prístup do exchangeovej poštovej schránky prostredníctvom webových služieb Exchangeu. Exchangeová poštová schránka môže byť online alebo lokálna. Ak sa online používateľom nezobrazuje karta Kalendár, uistite sa, že [majú licenciu na exchangeovú online poštovú schránku a poštová schránka je povolená](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Ak má používateľ platnú poštovú schránku v službe Exchange Online, ale stále sa nezobrazuje karta Kalendár, pravdepodobne sa vyskytol problém so sieťou. Použite [nástroj Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) a spustite **testovanie pripojenia vo webových službách Microsoft Exchangeu** pre daného používateľa.

Nakoniec skontrolujte [pre aplikácie Teams politiky nastavenia aplikácií](https://admin.teams.microsoft.com/policies/app-setup) a skontrolujte, či aplikácia Kalendár nebola odobratá z politiky, ktorá sa použila pre daného používateľa (s najväčšou pravdepodobnosťou sú to politiky **globálne (predvolené pre celú organizáciu)**.

Ak sú poštové schránky vašich používateľov lokálne, je potrebné potvrdiť, že je stav vašej hybridnej konfigurácie v poriadku. Ak chcete riešiť problémy, použite [Sprievodcu hybridnou konfiguráciou](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Upozorňujeme, že [aplikácia Teams vyžaduje Exchange 2016 CU3 alebo novší](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
