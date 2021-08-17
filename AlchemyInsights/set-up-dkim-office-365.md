---
title: Setup DKIM
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108571"
---
# <a name="setup-dkim"></a>Setup DKIM

Úplné pokyny na konfiguráciu DKIM pre vlastné domény v Microsoft 365 [tu.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Pre **každú** vlastnú doménu je potrebné vytvoriť dva **CNAME** záznamy DKIM u hostiteľských služieb DNS vašej domény (zvyčajne ide o registrátora domén). Napríklad contoso.com a fourthcoffee.com DKIM CNAME záznamy: dva pre contoso.com a dve pre fourthcoffee.com.

   CNAME záznamy DKIM pre **každú vlastnú** doménu používajú tieto formáty:

   - **Názov hostiteľa:**`selector1._domainkey.<CustomDomain>`

     Points to address or value : **(Odkazuje na adresu alebo hodnotu):**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   - **Názov hostiteľa:**`selector2._domainkey.<CustomDomain>`

     Points to address or value : **(Odkazuje na adresu alebo hodnotu):**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   \<DomainGUID\> je text naľavo od prispôsobeného záznamu MX pre vlastnú doménu (napríklad pre názov `.mail.protection.outlook.com` `contoso-com` domény contoso.com). \<InitialDomain\>je doména, ktorú ste použili pri Microsoft 365 konta (napríklad contoso.onmicrosoft.com).

2. Po vytvorení CNAME záznamov pre vlastné domény postupujte podľa týchto pokynov:

   a. [prihláste sa Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomocou svojho pracovného alebo školského konta.

   b. V ľavom hornom rohu vyberte ikonu spúšťača aplikácií a potom vyberte položku **Správca.**

   c. V navigácii v ľavom dolnom rohu rozbaľte **položku Správca** a vyberte **položku Exchange**.

   d. Prejdite na  >  **DKIM protection.**

   e. Vyberte doménu a potom vyberte položku **Povoliť pre podpisovanie** **správ pre túto doménu s podpismi DKIM**. Tento krok zopakujte pre každú vlastnú doménu.
