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
ms.openlocfilehash: f0f82eaaa00d71992af445bb89346fb85bad3ade5d120b25ad3a6ea4f9674893
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883334"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Chyba Základné pripojenie sa zavrelo v SharePoint

Ak sa zobrazí chyba "Základné pripojenie bolo zavreté" v programe SharePoint môže to súvisieť s nedostupním protokolu TLS 1.0/1.1. Ďalšie informácie nájdete v týchto článkoch:

- [Príprava na TLS 1.2 v Office 365 a Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Chyby overenia sa vyskytujú, ak klient nemá podporu protokolu TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Aktualizácia na povolenie protokolu TLS 1.1 a TLS 1.2 ako predvolených zabezpečených protokolov v systéme WinHTTP v Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ak sú používatelia v Windows 7, skontrolujte, či v protokole [TLS Cipher Suites Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)