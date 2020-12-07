---
title: Ikona kalendára sa nezobrazuje v klientovi Microsoft teams
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
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583926"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Ikona kalendára sa nezobrazuje v klientovi Microsoft teams

Karta **Kalendár** v aplikácii teams vyžaduje prístup k poštovej schránke programu Exchange prostredníctvom webových služieb Exchange Web Services. Poštová schránka Exchange môže byť online alebo lokálne. V prípade online používateľov, ktorí nezobrazujú kartu **Kalendár** , skontrolujte, či majú [licenciu na poštovú schránku služby Exchange Online a či je poštová schránka povolená](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Ak sú vaši používatelia doma lokálne, musíte potvrdiť, že vaša hybridná konfigurácia je zdravá. Ak chcete riešiť problémy, použite [Sprievodcu hybridnou konfiguráciou](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent). Upozorňujeme, že [aplikácia Teams vyžaduje Exchange 2016 CU3 alebo novší](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Ďalšie informácie a kroky na riešenie problémov nájdete v téme [Riešenie problémov s interakciou aplikácie Microsoft teams a Exchange servera](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
