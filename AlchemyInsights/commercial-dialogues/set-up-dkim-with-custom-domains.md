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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332322"
---
# <a name="set-up-dkim-with-custom-domains"></a>Nastavenie DKIM s vlastnými doménami

Musíte publikovať dva CNAME záznamy pre každú vlastnú doménu v DNS. Ak to chcete urobiť, použite nasledujúci formát:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Poznámka:** **DomainGUID** je text naľavo od **.mail.protection.outlook.com** vo prispôsobenom MX zázname pre vlastnú doménu (napríklad contoso-com pre **doménu contoso.com**). **InitialDomain** je doména, ktorú používate pri zaregistrovaní do Office 365 domény **(napríklad contoso.onmicrosoft.com**).

Ďalšie informácie o DNS záznamoch nájdete v téme Vytvorenie DNS záznamov pre všetky poskytovateľa [hostiteľských služieb Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)