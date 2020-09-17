---
title: Nastavenie DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808722"
---
# <a name="setup-dkim"></a>Nastavenie DKIM

Všetky pokyny na konfiguráciu DKIM pre vlastné domény v Microsoft 365 sú [tu](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Pre **každú** vlastnú doménu je potrebné vytvoriť **dva** CNAME záznamy CNAME na hostiteľskej službe DNS vašej domény (zvyčajne registrátora domén). Napríklad contoso.com a fourthcoffee.com vyžadujú štyri CNAME záznamy CNAME: dva pre contoso.com a dve pre fourthcoffee.com.

   CNAME CNAME záznamy pre **každú** vlastnú doménu používajú tieto formáty:

   - **Názov hostiteľa**: `selector1._domainkey.<CustomDomain>`

     **Odkazuje na adresu alebo hodnotu**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Názov hostiteľa**: `selector2._domainkey.<CustomDomain>`

     **Odkazuje na adresu alebo hodnotu**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je text naľavo od `.mail.protection.outlook.com` prispôsobeného MX záznamu pre vlastnú doménu (napríklad `contoso-com` pre doménu contoso.com). \<InitialDomain\> je doména, ktorú ste použili, keď ste sa zaregistrovali v službe Microsoft 365 (napríklad contoso.onmicrosoft.com).

2. Po vytvorení CNAME záznamov pre svoje vlastné domény postupujte podľa nasledujúcich pokynov:

   a. [Prihláste sa do služby Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomocou svojho pracovného alebo školského konta.

   b. V ľavom hornom rohu vyberte ikonu spúšťača aplikácií a vyberte položku **správca**.

   c. V navigácii v ľavom dolnom rohu rozbaľte položku **správca** a vyberte položku **Exchange**.

   d. Prejdite na **ochranu**  >  **dkim**.

   e. Vyberte doménu a potom vyberte položku **Povoliť** pre **podpísanie správ pre túto doménu pomocou podpisov dkim**. Zopakujte tento krok pre každú vlastnú doménu.
