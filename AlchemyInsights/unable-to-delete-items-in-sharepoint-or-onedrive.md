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
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049532"
---
# <a name="unable-to-delete-items"></a>Položky sa nedajú odstrániť

Máte problémy s odstránením položiek služby SharePoint?

- Vždy sa uistite, že máte [príslušné povolenia](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) na odstránenie položky alebo sa pokúsi odstrániť položku [správca kolekcie lokalít](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) .

- Uistite sa, že na položku nie je nastavenie [politiky uchovávania údajov](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .

- Uistite sa, že položka nie je [vzatý](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) k sebe inému používateľovi.

- Nakoniec, správcovia môžu používať [SharePoint vzory a postupy](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ktorý obsahuje knižnicu príkazov PowerShell, ktoré umožňujú vykonávať komplexné riadenie akcie, ako je sila odstránenie tvrdohlavý položky.
- [Odstrániť súbor PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Odstrániť priečinok PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Odstrániť položku zoznamu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Odstrániť zoznam PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Odstrániť pole PNP (stĺpec)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)