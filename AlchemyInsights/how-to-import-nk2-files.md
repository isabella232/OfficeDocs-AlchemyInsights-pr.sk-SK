---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043221"
---
# <a name="how-to-import-nk2-files"></a>Importovanie súborov .nk2 

Pri prvom spustení Microsoft Outlook 2013, Outlook 2016, Outlook 2019 alebo Outlook pre Microsoft 365 sa vyrovnávacia pamäť prezývk (uložená v súbore *profilename*.nk2) importuje do skrytej správy v predvolenom ukladaní správ.

Ak chcete importovať súbory .nk2 do služieb Outlook 2013, Outlook 2016, Outlook 2019 alebo Outlook pre Microsoft 365, skontrolujte, či sa súbor .nk2 nachádza v tomto priečinku: %appdata%\Microsoft\Outlook

**Poznámka:** Súbor .nk2 musí mať rovnaký názov ako aktuálny Outlook 2013 alebo Outlook 2016 profilu. Predvolene je názov profilu "Outlook". Ak chcete skontrolovať názov profilu, postupujte takto: 
1. Kliknite **na tlačidlo** Štart a potom kliknite na položku Ovládací **panel**.
2. Dvakrát kliknite na položku **Pošta.**
3. V dialógovom okne Nastavenie pošty vyberte položku **Zobraziť profily**.
4. Vyberte **položku Spustiť**  >  **Spustiť.**
5. Do poľa **Otvoriť** zadajte príkaz *outlook.exe /importnk2 a* potom vyberte tlačidlo **OK**. 

Po importe súboru .nk2 sa obsah súboru zlúči do existujúcej vyrovnávacej pamäte prezývk, ktorá je uložená vo vašej poštovej schránke.

**Poznámka:** Súbor .nk2 sa premenuje na príponu .old pri najbližšom spustení programu Outlook 2013, Outlook 2016, Outlook 2019 alebo Outlook pre Microsoft 365. Ak chcete súbor .nk2 znova importovať, odstráňte najprv príponu .old.

Ďalšie informácie nájdete v téme [Import alebo kopírovanie zoznamu automatického dokončovania do iného počítača.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)