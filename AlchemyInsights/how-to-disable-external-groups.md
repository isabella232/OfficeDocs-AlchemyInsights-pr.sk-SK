---
title: Ako zakázať externé skupiny
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384840"
---
# <a name="how-to-disable-external-groups"></a>Ako zakázať externé skupiny

Yammer externých správ sa uplatňuje Exchange Transport pravidlá (Red), sadu aktívne kontroly na zabrániť zdieľaniu informácií spoločnosti. S cieľom obmedziť používateľov od vytvorenia externé skupiny, musíte nakonfigurovať výmena pravidlo prenosu (ETR), a potom nakonfigurovať sieť Yammer používať Exchange dopravné pravidlo blokovať externých správ.
  
Akonáhle ste vytvorili pravidlo Exchange Online admin Center, postupujte nasledovne nastaviť ETR použiť v sieť Yammer:
  
- Prihlásenie na sieť Yammer len overené a **Yammer admin center**, prejdite na C **obsahu a zabezpečenia \> nastavenia zabezpečenia.**

- Podľa **Externých správ**, vyberte **presadiť vaše Exchange Online Exchange Transport pravidlá (Red) v nariekanie.**

- Vyberte položku **Uložiť**.

Ďalšie informácie nájdete v téme [kontroly externých správ v sieti sieť Yammer s Exchange Transport pravidlá](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)
  