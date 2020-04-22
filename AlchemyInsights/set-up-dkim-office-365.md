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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645687"
---
# <a name="setup-dkim"></a>Nastavenie DKIM

Kompletné pokyny pre konfiguráciu DKIM pre vlastné domény v Microsoft 365 sú [tu](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Pre **každú** vlastnú doménu, musíte vytvoriť **dva** dkim CNAME záznamy v doméne DNS hostingové služby (typicky, Registrátor domén). Napríklad contoso.com a fourthcoffee.com vyžadujú štyri záznamy DKIM CNAME: dve pre contoso.com a dve pre fourthcoffee.com.

   Záznamy CNAME DKIM pre **každú** vlastnú doménu používajú nasledujúce formáty:

   - **Názov hostiteľa**:`selector1._domainkey.<CustomDomain>`

     **Body na adresu alebo hodnotu**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Názov hostiteľa**:`selector2._domainkey.<CustomDomain>`

     **Body na adresu alebo hodnotu**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je text naľavo `.mail.protection.outlook.com` v prispôsobenom zázname MX pre vlastnú doménu (napríklad `contoso-com` pre doménu contoso.com). \<InitialDomain\> je doména, ktorú ste použili pri prihlásení do spoločnosti Microsoft 365 (napríklad contoso.onmicrosoft.com).

2. Po vytvorení záznamov CNAME pre vlastné domény postupujte podľa nasledujúcich pokynov:

   A. [Prihláste sa do Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) so svojím pracovným alebo školským kontom.

   B. V ľavom hornom rohu vyberte ikonu spúšťača aplikácií a vyberte možnosť **správca**.

   C. V ľavom dolnom navigáciu, rozbaľte **admin** a vyberte **Exchange**.

   D. Prejdite na **ochranu** > **dkim**.

   E. Vyberte doménu a potom vyberte **Povoliť** pre **podpísať správy pre túto doménu s dkim podpisy**. Zopakujte tento krok pre každú vlastnú doménu.
