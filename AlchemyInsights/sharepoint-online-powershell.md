---
title: SharePoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764276"
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