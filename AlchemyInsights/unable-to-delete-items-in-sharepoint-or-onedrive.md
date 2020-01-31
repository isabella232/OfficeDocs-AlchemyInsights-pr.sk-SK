---
title: Nie je možné odstrániť položky v službe SharePoint alebo OneDrive
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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571286"
---
# <a name="unable-to-delete-items"></a>Položky sa nedajú odstrániť

Politiky uchovávania údajov môžu spôsobiť to, musíte buď vypnúť alebo vylúčiť príslušné zadržanie, ktoré spôsobuje tento problém. Po odstránení politiky uchovávania alebo zadržania môže zmena trvať až 24 hodín. Uistite sa, že na položku nie je nastavenie [politiky uchovávania údajov](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .

Lokalita mohla prekročiť limit ukladacieho priestoru, zvýšiť [kvótu lokality](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) a odstrániť položku.

Uistite sa, že položka nie je [vzatý](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) k sebe inému používateľovi.

Nakoniec, správcovia môžu používať [SharePoint vzory a postupy](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ktorý obsahuje knižnicu príkazov PowerShell, ktoré umožňujú vykonávať komplexné riadenie akcie, ako je sila odstránenie tvrdohlavý položky.
- [Odstrániť súbor PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odstrániť priečinok PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odstrániť položku zoznamu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odstrániť zoznam PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odstrániť pole PNP (stĺpec)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)