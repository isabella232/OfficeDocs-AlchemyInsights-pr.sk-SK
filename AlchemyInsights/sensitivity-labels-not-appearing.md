---
title: Označenia citlivosti, ktoré sa nezobrazujú
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207240"
---
# <a name="sensitivity-labels-not-appearing"></a>Označenia citlivosti, ktoré sa nezobrazujú

Štítky citlivosti vám umožňujú klasifikovať a chrániť citlivý obsah. Môžu byť vytvorené v Microsoft 365 Compliance Center, Microsoft 365 centrum zabezpečenia alebo Office 365 zabezpečenia & Compliance Center podľa klasifikácie > citlivosť menovky. Ďalšie informácie o tejto funkcii nájdete v téme [Prehľad označení citlivosti](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).

Ak ste nakonfigurovali menovky citlivosti, ale nezobrazujú sa v aplikáciách balíka Office, skontrolujte nasledovné:

- Potvrďte, že štítok citlivosti bol [publikovaný](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) pre používateľov a skupiny, ktoré chcete.

- Potvrďte, že používateľ používa aplikáciu, ktorá podporuje menovky citlivosti – Pozrite si [menovky citlivosti v dokumente](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Ak [migrujete štítky na ochranu informácií Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), uvedomte si [tu](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)uvedené úvahy.

- Podpora ochrany pred únikom údajov (DLP): v súčasnosti môžu byť v politikách DLP použité len menovky uchovávania.  Podpora pre označenia citlivosti v politike DLP nie je zatiaľ k dispozícii, ale pracujeme na tom.

- Ak je šifrovanie zapnuté na štítku citlivosti, môžete vybrať buď:
    - Priradiť povolenia teraz
    - Umožniť používateľom priraďovať povolenia


Ďalšie informácie o možných problémoch nájdete v téme [známe problémy s menovkami citlivosti](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).