---
title: Oneskorenie pri prijímaní upozornení SharePointu a OneDrivu
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
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727258"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Oneskorenie pri prijímaní upozornení SharePointu a OneDrivu

- Najskôr skontrolujte priečinok nevyžiadanej pošty alebo Nevyžiadaná pošta v e-maile.
- Ak **sú všetky upozornenia z viacerých súborov alebo knižníc oneskorené**, navštívte [tabuľu stavu služby](https://portal.office.com/adminportal/home?ref=/servicehealth) a skontrolujte, či sú k dispozícii upozornenia alebo incidenty, ktoré sa môžu vyskytnúť v SharePointe alebo Exchangei. Problém môže byť s funkciou upozornenia SharePointu alebo oneskorením v e-mailoch cez Exchange. Všimnite si tiež, či sa doručujú iné e-maily – Ak nie, problém je pravdepodobne s oneskorením pri výmene.
- Ak **sa nedoručuje individuálne upozornenie zo špecifického súboru alebo knižnice**, pokúste sa ho odstrániť a znova vytvoriť. Ďalšie informácie o opätovnom vytvorení upozornenia nájdete v téme [Správa, zobrazenie alebo odstránenie upozornení SharePointu](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .

> [!NOTE]
> - Upozornenia nie je možné odoslať do distribučnej skupiny. Podporované sú len skupiny zabezpečenia a služby O365.
> - Nie je možné prispôsobiť šablóny upozornení e-mailom. Na dosiahnutie týchto úloh je nutné použiť pracovný postup Microsoft Flow alebo SharePoint Designer.
