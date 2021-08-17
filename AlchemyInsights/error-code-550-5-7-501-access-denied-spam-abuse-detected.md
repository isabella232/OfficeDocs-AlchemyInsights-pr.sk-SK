---
title: Kód chyby 550 5.7.501 Prístup odmietnutý, zistené zneužitie nevyžiadanej pošty
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: a3eebe4e9d69e100a750e74a6d34ec67dc0566df5dd6eb59809adb07ed8a682f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044283"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 Prístup odmietnutý, zistené zneužitie nevyžiadanej pošty

Toto hlásenie sa zvyčajne zobrazí, keď používatelia odošlú e-mailové správy z IP adries pomocou počiatočnej domény *.onmicrosoft.com,* ktorá je priradená novým nájomníkom v Microsoft 365. Najjednoduchším spôsobom riešenia tohto problému je:

1. [Pridajte doménu k nájomníkovi](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).

2. [Zmeňte primárnu e-mailovú adresu používateľa](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) na novú vlastnú doménu, ktorú ste práve pridali.
