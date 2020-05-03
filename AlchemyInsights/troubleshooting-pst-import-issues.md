---
title: Riešenie problémov s importom súborov PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991381"
---
# <a name="troubleshooting-pst-import-issues"></a>Riešenie problémov s importom súborov PST

- Ak importujete v samotnom klientovi Outlook, prečítajte si tému [Riešenie problémov s importovaním súboru .pst programu Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Ak používate službu Import Service a zasekla sa, nezabúdajte, že žiadny súbor PST, ktorý nahráte do ukladacieho priestoru platformy Azure, by nemal byť väčší ako 20 GB. Súbory PST väčšie ako 20 GB môžu mať vplyv na výkon procesu importu súborov PST.

- Ak chcete overiť stav konkrétnej úlohy importu, môžete použiť [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Podrobné informácie o službe importu nájdete v téme [Prehľad importovania súborov PST vašej organizácie](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
