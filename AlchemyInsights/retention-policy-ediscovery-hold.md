---
title: 2609-zadržanie-alebo-eDiscovery-hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994094"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>Nie je možné odstrániť položky SharePoint Online alebo OneDrive pre podniky

Vy alebo vaši používatelia môžu byť schopní odstrániť položky SharePoint Online alebo OneDrive pre podniky, pretože politika uchovávania údajov, označenie uchovávania údajov alebo eDiscovery hold sa aplikuje na SharePoint OneDrive lokality alebo konkrétnu položku. Toto zahŕňa možnosť odstránenia dokumentu, verzie dokumentu, priečinka, knižnice dokumentov, zoznamu, aplikácie, lokality alebo kolekcie lokalít. Tu je niekoľko príkladov chybových hlásení, ktoré sa môžu prijímať pri pokuse o odstránenie položky, ktorá sa zachová:

- "Táto stránka nemôže byť odstránená, pretože je zahrnutá v eDiscovery zadržanie alebo politiky uchovávania údajov"
- "Táto stránka má politiku súladu nastaviť blokovať odstránenie"
- "Politika súladu je v súčasnosti blokuje odstránenie tejto lokality"
- "Táto kolekcia lokalít nie je možné odstrániť, pretože obsahuje lokality, ktoré sú súčasťou eDiscovery zadržanie alebo politiky uchovávania údajov"
- "Musíte odstrániť všetky položky v tomto priečinku pred odstránením priečinka"
- "Verzie tejto položky nie je možné odstrániť, pretože je v zadržanie alebo politika uchovávania údajov"
- "Položka sa nedá odstrániť počas podržania"
- "Štítok, ktorý sa aplikuje na túto položku zabraňuje jeho úprave alebo odstráneniu"
- "Zoznam nie je možné odstrániť pri podržaní alebo uchovávania politiky"
- "Zoznam nie je možné odstrániť, ak je blokovaný alebo ak politika uchovávania údajov je použitá na to"

Ak chcete odstrániť položky v jednom z týchto scenárov, musí sa odstrániť politika uchovávania údajov, štítok uchovávania údajov alebo zadržanie eDiscovery (alebo lokalita musí byť vylúčená z politiky uchovávania údajov). Musíte buď vypnúť alebo vylúčiť príslušné držanie, ktoré spôsobuje tento problém. Po odstránení politiky uchovávania alebo zadržania môže zmena trvať až 24 hodín. 

Ďalšie informácie o rôznych funkciách uchovávania a zadržania, ktoré možno aplikovať na lokality SharePoint a kontá OneDrive, nájdete v niektorej z nasledujúcich tém.

- [Prehľad politík uchovávania údajov](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [Prehľad štítkov uchovávania údajov](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [Správa drží v pokročilom eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [eDiscovery drží](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [Staršie politiky uzavretia a odstránenia lokality](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
