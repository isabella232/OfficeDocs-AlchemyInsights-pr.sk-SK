---
title: Problémy s SharePoint v Windows 7
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
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125517"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Problémy s SharePoint v Windows 7

Ak sa pri práci so systémom SharePoint alebo OneDrive v počítačoch Windows 7 zobrazí chyba, môžu súvisieť s tým, že sa zrušia protokol TLS 1.0/1.1. Ďalšie informácie nájdete v téme:

- [Príprava na TLS 1.2 v Office 365 a Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 klienti musia mať povolený protokol TLS1.2. Ďalšie informácie nájdete v téme [Chyby overenia sa vyskytujú, keď klient nemá podporu protokolu TLS 1.2.](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Nainštalujte KB3140245 a vytvorte hodnotu databázy Registry. Ďalšie informácie nájdete v téme Aktualizácia na povolenie [TLS 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) ako predvolených zabezpečených protokolov vo WinHTTP v Windows

- Windows 7 SP1/Windows 8 klienti musia zabezpečiť inštaláciu najnovších šifrovaných objektov TLS. Ďalšie informácie nájdete v téme [Microsoft Security Advisory 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


