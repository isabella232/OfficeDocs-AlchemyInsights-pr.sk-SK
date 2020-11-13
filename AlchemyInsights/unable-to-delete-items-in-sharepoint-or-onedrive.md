---
title: Nie je možné odstrániť položky v SharePointe alebo vo OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019598"
---
# <a name="unable-to-delete-items"></a>Nie je možné odstrániť položky

- Politiky uchovávania údajov môžu spôsobiť, že je potrebné vypnúť alebo vylúčiť príslušné zadržanie, ktoré spôsobuje tento problém. Po odstránení politiky alebo zadržania uchovávania údajov môže zmena nadobudnúť až 24 hodín. Skontrolujte, či sa v položke nenachádza nastavenie [politiky uchovávania údajov](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) .

- Lokalita mohla prekročila limit ukladacieho priestoru, zvýšiť [kvótu lokality](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) a odstrániť ju.

- Uistite sa, že položka nie je [vzatá z projektu](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) inému používateľovi.

- Správcovia môžu nakoniec použiť [vzorce a postupy SharePointu](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ktoré obsahujú knižnicu príkazov prostredia PowerShell, ktoré vám umožňujú vykonávať zložité akcie spravovania, ako je napríklad vynútiť odstraňovanie nepoddajných položiek.
- [Odstránenie súboru PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odstránenie priečinka PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odstránenie položky zoznamu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odstrániť zoznam PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odstrániť pole PNP (stĺpec)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)