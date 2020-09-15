---
title: Zakázanie externých skupín
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704143"
---
# <a name="how-to-disable-external-groups"></a>Zakázanie externých skupín

Externé správy v Yammeri používajú pravidlá prenosu systému Exchange (ETRs), množinu proaktívnych ovládacích prvkov, aby sa predišlo zdieľaniu informácií o spoločnosti. Ak chcete obmedziť používateľov na vytváranie externých skupín, musíte nakonfigurovať pravidlo prenosu služby Exchange (ETR) a potom nakonfigurovať Yammer na blokovanie externých správ pomocou pravidla prenosu Exchangeu.
  
Po vytvorení pravidla v centre spravovania služby Exchange Online postupujte podľa týchto krokov na nastavenie ETR na použitie v Yammeri:
  
- Prihláste sa do Yammera ako overený správca a v **centre spravovania služby Yammer**prejdite na **položky C obsah a zabezpečenie zabezpečenia \> .**

- V časti **externé správy**vyberte **v Yammeri položku vynútiť pravidlá prenosu Exchange Online Exchange (ETRs).**

- Vyberte položku **Uložiť**.

Ďalšie informácie nájdete v téme [Vypnutie externých správ v sieti Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  