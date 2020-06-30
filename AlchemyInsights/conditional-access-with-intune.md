---
title: Podmienený prístup pomocou služby Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931451"
---
# <a name="conditional-access-with-intune"></a>Podmienený prístup pomocou služby Intune

Použitie **podmieneného prístupu** pomocou služby Intune vyžaduje 3 kroky:

- Vytvorte **politiku súladu** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) na definovanie nastavení, ktoré musia byť splnené pred tým, ako sa zariadenie považuje za kompatibilné. Zariadenie musí mať napríklad špendlík s číslom najmenej 6 číslic predtým, ako sa považuje za vyhovujúce.
- Vytvorte **politiku podmieneného prístupu,** ktorá definuje, ktoré zdroje sú chránené a aké podmienky je potrebné splniť na prístup k týmto prostriedkom.  [Zariadenie](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) musí byť napríklad kompatibilné pred prístupom k podnikovým e-mailom.
- Zabezpečte, aby boli **politiky súladu** aj **politiky podmieneného prístupu** zacielené na požadované skupiny používateľov. To môže vyžadovať vytvorenie konkrétnych skupín používateľov v službe Azure Active Directory.

**Užitočné odkazy:**

[Prehľad súladu zariadenia](https://docs.microsoft.com/intune/device-compliance-get-started)

[Riešenie problémov CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Politika riešenia problémov](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Na ochranu e-mailu (Exchange online) pred prístupom nevyhovujúcich zariadení, oba dokumenty musia byť dodržiavané:

1. [Ochrana prístupu k e-mailu zo zariadení pomocou EAs](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Chráňte prístup k e-mailom zo zariadení pomocou moderných klientov overovania, ako je napríklad Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)