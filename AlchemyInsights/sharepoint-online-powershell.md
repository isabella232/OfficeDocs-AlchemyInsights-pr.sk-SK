---
title: SharePoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123013"
---
# <a name="sharepoint-online-powershell"></a>SharePoint Online PowerShell

Práca s PowerShell alebo skripty v rámci SharePoint Online? Ďalšie informácie nájdete na nižšie uvedených odkazoch.
- [Začíname pracovať s SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Pripojenie k SPO PowerShell s multifaktorové overovanie (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint vzory a postupy (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) obsahuje knižnicu príkazov PowerShell, ktoré vám umožní vykonávať komplexné riadenie činnosti voči spo.

> [!NOTE]
> - Ak máte problémy s pripojením k správe SPO Management Shell, uistite sa, že ste aktualizovali na najnovšiu verziu a pokúste sa [znova importovať modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) pomocou *"Import-module Microsoft. online. SharePoint. PowerShell".*
> - Ak sa pokúšate spustiť klientske skripty objektového modelu, budete musieť mať [SharePoint Online client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) nainštalovaný na lokálnom počítači.
> - Ak máte problémy so spustením skriptov z PowerShell, možno budete chcieť zvážiť spustenie PowerShell ako správca a zmena [vykonávania politiky](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).