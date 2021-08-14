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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972434"
---
# <a name="troubleshooting-pst-import-issues"></a>Riešenie problémov s importom súborov PST

- Ak importujete v rámci samotného Outlook klienta, pozrite si [časť Riešenie problémov s importom Outlook .pst.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Ak používate službu importovania a zasekla sa, každý súbor PST, ktorý nahráte do ukladacieho priestoru platformy Azure, by nemal byť väčší ako 20 GB. Pst súbory väčšie ako 20 GB môžu mať vplyv na výkon procesu importu PST. Ďalšie informácie o riešení problémov s uviaznutými úlohami nájdete [v téme Problémy, ktoré majú vplyv na úlohy importu PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Ak chcete overiť stav konkrétnej úlohy importu, použite rutinu [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Úplné podrobnosti o službe importovania nájdete v [téme Prehľad importovania súborov PST organizácie.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
