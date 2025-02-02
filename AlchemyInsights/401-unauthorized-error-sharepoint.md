---
title: 401 Neoprávnená chyba vo SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 04f56dfc7ebe7de91bc64a5e6d2b480b07741c6e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314363"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Neoprávnená chyba vo SharePoint

Ak sa v programe SharePoint zobrazí chybové hlásenie "(401) Neoprávnené, môže to súvisieť s nedostupním protokolu TLS 1.0/1.1. Ďalšie informácie nájdete v témach:

- [Príprava na TLS 1.2 v Office 365 a Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Chyby overenia sa vyskytujú, ak klient nemá podporu protokolu TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Aktualizácia na povolenie protokolu TLS 1.1 a TLS 1.2 ako predvolených zabezpečených protokolov v winhttps://support.microsoft.com/Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Ak sú používatelia v Windows 7, uistite sa, že zadýchnú [šifrovanie TLS v Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)