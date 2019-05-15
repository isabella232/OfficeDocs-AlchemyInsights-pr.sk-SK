---
title: Nepodarilo sa odstrániť položky v SharePoint alebo OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057772"
---
# <a name="unable-to-delete-items"></a>Nemožno odstrániť položky

Problémy s odstránením položiek?

- Vždy skontrolujte, či máte [príslušné povolenia](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) na odstrániť položku alebo mať [správca kolekcie lokality](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) pokus odstrániť položku.

- Uistite sa, že nie je nastavenie [politiky uchovávania údajov](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) položky.

- Uistite sa, či položka nie je [vzatý k sebe](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) iný používateľ.

- Napokon, správcovia môžu pomocou [SharePoint vzorov a postupov](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ktorý obsahuje knižnicu PowerShell príkazy, ktoré vám umožnia vykonávať komplexné riadenie činnosti, ako napríklad sila odstránenie tvrdohlavý položiek. 
- [Odstrániť PNP súbor](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odstrániť priečinok PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odstrániť položku PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odstrániť PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odstrániť PNP pole (stĺpec)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)