---
title: Nastavenie DKIM v balíku Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765407"
---
# <a name="setup-dkim-in-office-365"></a>Nastavenie DKIM v balíku Office 365

Úplné pokyny na konfigurovanie DKIM vlastnej domény v Office 365 sú [tu](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Pre **každú** vlastnú doménu, musíte vytvoriť **dva** záznamy DKIM CNAME hostiteľskej služby servera DNS vašej domény (zvyčajne Registrátor domén). Napríklad contoso.com a fourthcoffee.com vyžadujú štyri DKIM CNAME záznamov: dva pre contoso.com a dva pre fourthcoffee.com.

   DKIM CNAME záznamov pre **každú** vlastnú doménu, použite nasledujúce formáty:

   - **Názov hostiteľa**:`selector1._domainkey.<CustomDomain>`

     **Body na adresu alebo hodnotu**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Názov hostiteľa**:`selector2._domainkey.<CustomDomain>`

     **Body na adresu alebo hodnotu**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je text naľavo od `.mail.protection.outlook.com` v prispôsobených záznam MX pre domény (napríklad `contoso-com` domény contoso.com). \<InitialDomain\> je doména, ktorú ste použili pri registrácii do služby Office 365 (doménu napríklad contoso.onmicrosoft.com).

2. Po vytvorení záznamy CNAME pre svoje vlastné domény, použite nasledujúce pokyny:

   a. [Prihlásenie do služby Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomocou konta práca alebo škola.

   b. Vyberte ikonu launcher aplikácie v ľavom hornom a **Admin**.

   c. V ľavom dolnom navigácia, rozbaľte **Admin** a vyberte **Exchange**.

   d. Prejdite na **ochranu** > **DKIM**.

   e. Vyberte doménu, a potom vyberte **Povoliť** pre **znak správy pre túto doménu s podpismi DKIM**. Zopakujte tento krok pre každú vlastnú doménu.
