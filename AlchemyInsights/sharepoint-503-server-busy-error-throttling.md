---
title: SharePoint Online obmedzovanie
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751903"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online obmedzovanie

Používatelia môžu získať 503 server je zaneprázdnený chyba pri pokuse o navigáciu na lokality SharePoint alebo OneDrive. 

Táto chyba môže byť spôsobená škrtenia v službe SharePoint. SharePoint Online používa obmedzovanie zachovať optimálny výkon a spoľahlivosť služby SharePoint Online. Obmedzovanie obmedzuje počet používateľských akcií alebo súbežné volania (podľa skriptu alebo kódu), aby sa zabránilo nadvyužívaniu zdrojov. Ak sa vám škrtil, 99% času je to preto, že vlastný kód.

Ďalšie informácie o obmedzovanie vidieť, [vyhnúť sa škrtil alebo blokované SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Ak sa domnievate, že táto chyba nesúvisí s škrtenia, môžete skontrolovať, či je aktívna údržba, ktorá sa vyskytuje na nájomníkovi, a to tak, že prejdete do [centra správ](https://portal.office.com/adminportal/home#/MessageCenter).

 Nakoniec, uistite sa, že navštívite stránku [služby zdravie](https://portal.office.com/adminportal/home#/servicehealth) skontrolovať všetky upozornenia/incidenty, ktoré môžu byť vyskytujúce.

