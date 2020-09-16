---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770854"
---
# <a name="sharepoint-online-powershell"></a>SharePoint Online PowerShell

Pracujete s prostredím PowerShell alebo skriptami v SharePointe Online? Ďalšie informácie nájdete na prepojeniach nižšie.
- [Začíname so službou SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Pripojenie k službe SPO PowerShell s overovaním multifacto (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [Šablóny a postupy SharePointu (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) obsahujú knižnicu príkazov prostredia PowerShell, ktoré vám umožňujú vykonávať komplexné manažérske akcie na spo.

> [!NOTE]
> - Ak máte problémy s pripojením k shellu riadenia SPO, uistite sa, že ste aktualizovali na najnovšiu verziu a pokúsite sa [znova importovať modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) pomocou *"Import-module Microsoft. online. SharePoint. PowerShell".*
> - Ak sa pokúšate spustiť skripty objektového modelu na strane klienta, bude potrebné, aby ste mali v lokálnom počítači nainštalovanú [súpravu SDK pre klientske súčasti SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) .
> - Ak máte problémy so spustením skriptov z prostredia PowerShell, môžete zvážiť spustenie prostredia PowerShell ako správca a zmeniť [politiku vykonávania](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).