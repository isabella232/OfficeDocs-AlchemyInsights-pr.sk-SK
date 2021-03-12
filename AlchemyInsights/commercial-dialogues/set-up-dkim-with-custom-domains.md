---
title: Nastavenie DKIM s vlastnými doménami
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747637"
---
# <a name="set-up-dkim-with-custom-domains"></a>Nastavenie DKIM s vlastnými doménami

Pre každú vlastnú doménu v službe DNS musíte publikovať dva CNAME záznamy. Ak to chcete urobiť, použite nasledujúci formát:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** je text naľavo od **. mail.Protection.Outlook.com** v prispôsobenom MX zázname pre vlastnú doménu (napríklad contoso-com pre doménu **contoso.com**). **InitialDomain** je doména, ktorú ste použili pri registrácii v službách Office 365 (napríklad **contoso.onmicrosoft.com**).

Ďalšie informácie o DNS záznamoch nájdete [v téme Vytvorenie záznamov DNS u ktoréhokoľvek poskytovateľa hostiteľských služieb DNS pre Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).