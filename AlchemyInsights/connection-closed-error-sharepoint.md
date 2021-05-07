---
title: Základné pripojenie sa v programe SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233441"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Chyba Základné pripojenie sa zavrelo v SharePoint

Ak sa zobrazí chyba "Základné pripojenie bolo zavreté" v SharePoint môže to súvisieť s nedostupním protokolu TLS 1.0/1.1. Ďalšie informácie nájdete v týchto článkoch:

- [Príprava na TLS 1.2 v Office 365 a Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [Chyby overenia sa vyskytujú, ak klient nemá podporu protokolu TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Ak sú používatelia v Windows 7, skontrolujte, či zadýchli [šifrovanie TLS v Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)