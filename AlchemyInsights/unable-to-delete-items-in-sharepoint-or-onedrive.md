---
title: Nie je možné odstrániť položky v SharePointe alebo OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511991"
---
# <a name="unable-to-delete-items"></a>Nie je možné odstrániť položky

Politiky uchovávania údajov môže spôsobiť, musíte vypnúť alebo vylúčiť príslušné zadržanie, ktoré spôsobuje tento problém. Po odstránení politiky uchovávania údajov alebo zadržaní môže trvať až 24 hodín, kým sa zmena prejaví. Skontrolujte, či v položke nie je nastavenie [politiky uchovávania údajov.](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

Lokalita mohla prekročiť limit ukladacieho priestoru, zvýšiť [kvótu lokality](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) a odstrániť položku.

Skontrolujte, či položka nie je [vzatá k sebe](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) inému používateľovi.

Nakoniec správcovia môžu používať [SharePoint vzory a postupy](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ktorý obsahuje knižnicu príkazov prostredia PowerShell, ktoré umožňujú vykonávať zložité akcie správy, ako je napríklad vynútenie odstránenia tvrdohlavých položiek.
- [Odstrániť pnp súbor](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odstrániť pnp priečinok](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odstrániť položku zoznamu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odstrániť pnp zoznam](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odstrániť pole PNP (stĺpec)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)