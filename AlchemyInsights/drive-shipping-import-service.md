---
title: Odoslanie disku v službe Microsoft 365 Import Service
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731947"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Odoslanie disku v službe Microsoft 365 Import Service

Pomocou odosielania disku skopírujte súbory PSTs na pevný disk a potom pevný disk odovedzte spoločnosti Microsoft.

Začatie úlohy:

1. V centre Microsoft 365 dodržiavania súladu v časti **Riadenie informácií** vyberte položku **Importovať**.

1. Vyberte **položku Vyberte typ úlohy importu** a potom vyberte položku **Ďalej**.

1. Ak chcete zobraziť postup pre túto možnosť importu, vyberte **položku Pevný disk do niektorého z našich fyzických umiestnení.**

Tu je niekoľko vecí, na ktoré je potrebné pamätať:

- Ak chcete v poštovej schránke importovať súbory PST do poštových schránok, Exchange Online mať priradenú rolu importu a exportu Microsoft 365 poštovej schránky.
Výkon môže ovplyvniť viac ako 20 GB v prípade PT, ktoré sú väčšie.

- Podporované sú len 2,5-palcové SSD disky alebo 2,5-palcové alebo 3,5-palcové interné pevné disky SATA II/III.
Pevný disk obsahujúci súbory PST musí byť zašifrovaný šifrovanie BitLocker.

- Poplatok za importovanie súborov PST do Microsoft 365 poštových schránok pomocou odosielania disku je 2 USD za každý GB údajov.

Ďalšie informácie o používaní spôsobu odosielania disku na importovanie súborov PST nájdete v téme Importovanie súborov PST organizácie [pomocou odosielania disku.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)