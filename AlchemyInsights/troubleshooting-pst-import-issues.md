---
title: Riešenie problémov s importom súborov PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826178"
---
# <a name="troubleshooting-pst-import-issues"></a>Riešenie problémov s importom súborov PST

- Ak importujete v samotnom klientovi Outlook, prečítajte si tému [Riešenie problémov s importovaním súboru .pst programu Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Ak používate službu Import Service a zasekla sa, nezabúdajte, že žiadny súbor PST, ktorý nahráte do ukladacieho priestoru platformy Azure, by nemal byť väčší ako 20 GB. Súbory PST väčšie ako 20 GB môžu mať vplyv na výkon procesu importu súborov PST.

- Ak chcete overiť stav konkrétnej úlohy importu, môžete použiť [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Podrobné informácie o službe importu nájdete v téme [Prehľad importovania súborov PST vašej organizácie](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
