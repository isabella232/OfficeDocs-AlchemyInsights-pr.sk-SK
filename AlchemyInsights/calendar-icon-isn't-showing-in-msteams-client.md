---
title: Ikona kalendára sa nezobrazuje v Microsoft Teams klientovi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120019"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Ikona kalendára sa nezobrazuje v Microsoft Teams klientovi

Karta **Kalendár** v Teams vyžaduje prístup k poštovej schránke Exchange cez Exchange Web Services. Poštová Exchange môže byť online alebo lokálna. Používateľom online, ktorí kartu  Kalendár nemajú, skontrolujte, či majú licenciu na poštovú schránku služby Exchange Online a či [je poštová schránka povolená.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) Ak sú vaši používatelia v domácnosti lokálne, musíte potvrdiť, že vaša hybridná konfigurácia je v poriadku. Ak chcete riešiť problémy, použite [Sprievodcu hybridnou konfiguráciou](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent). Upozorňujeme, že [aplikácia Teams vyžaduje Exchange 2016 CU3 alebo novší](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Ďalšie informácie a kroky na riešenie problémov nájdete v [téme Riešenie Microsoft Teams problémov Exchange Server s interakciou.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
