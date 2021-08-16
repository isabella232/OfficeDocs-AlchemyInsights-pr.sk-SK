---
title: Nie je možné odstrániť položky vo SharePoint alebo OneDrive
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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038532"
---
# <a name="unable-to-delete-items"></a>Nie je možné odstrániť položky

- Politiky uchovávania údajov to môžu spôsobiť, je potrebné zakázať alebo vylúčiť príslušné zadržanie, ktoré tento problém spôsobuje. Po odstránení politiky uchovávania údajov alebo zadržania môže trvať až 24 hodín, kým sa zmena prejaví. Skontrolujte, či pre položku neexistuje [nastavenie](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) politiky uchovávania údajov.

- Lokalita pravdepodobne prekročila limit ukladacieho priestoru, zväčší [kvótu lokality](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) a odstráni položku.

- Skontrolujte, či položka nie je [vzatá z](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) sebe inému používateľovi.

- Nakoniec môžu správcovia použiť [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ktorá obsahuje knižnicu príkazov prostredia PowerShell, ktoré vám umožňujú vykonávať zložité akcie správy, ako je napríklad vynútenie odstránenia ťažko odstránia ťažko odstránianých položiek.
- [Odstránenie súboru PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odstránenie priečinka PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odstránenie položky zoznamu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odstránenie zoznamu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odstránenie poľa PNP (stĺpca)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)