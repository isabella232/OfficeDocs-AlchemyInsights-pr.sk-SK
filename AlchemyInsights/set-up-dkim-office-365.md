---
title: Nastavenie DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509399"
---
# <a name="setup-dkim"></a>Nastavenie DKIM

Kompletné pokyny pre konfiguráciu DKIM pre vlastné domény v Microsoft 365 sú [tu](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Pre **každú vlastnú** doménu je potrebné vytvoriť **dva** záznamy DKIM CNAME v hostiteľskej službe DNS vašej domény (zvyčajne registrátordomény). Napríklad contoso.com a fourthcoffee.com vyžadujú štyri záznamy DKIM CNAME: dva pre contoso.com a dva pre fourthcoffee.com.

   Záznamy DKIM CNAME pre **každú** vlastnú doménu používajú nasledujúce formáty:

   - **Názov hostiteľa**:`selector1._domainkey.<CustomDomain>`

     **Počet bodov na adresu alebo hodnotu:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Názov hostiteľa**:`selector2._domainkey.<CustomDomain>`

     **Počet bodov na adresu alebo hodnotu:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>je text naľavo `.mail.protection.outlook.com` od prispôsobeného záznamu MX pre vlastnú doménu (napríklad `contoso-com` pre contoso.com domény). \<InitialDomain\>je doména, ktorú ste použili pri registrácii v programe Microsoft 365 (napríklad contoso.onmicrosoft.com).

2. Po vytvorení cname záznamov pre vlastné domény, postupujte podľa nasledujúcich pokynov:

   a. [prihláste sa do služby Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomocou pracovného alebo školského konta.

   b. V ľavom hornom rohu vyberte ikonu spúšťača aplikácií a vyberte **položku Správca**.

   c. V ľavom dolnom paneli rozbaľte položku **Správca** a vyberte položku **Exchange**.

   D. Prejsť na **Ochrana**  >  **DKIM**.

   E. Vyberte doménu a potom vyberte **položku Povoliť** **pre podpisy pre túto doménu s podpismi DKIM**. Zopakujte tento krok pre každú vlastnú doménu.
