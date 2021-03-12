---
title: Používanie podmieneného prístupu so službou Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749262"
---
# <a name="using-conditional-access-with-intune"></a>Používanie podmieneného prístupu so službou Intune

Používanie podmieneného prístupu so službou Intune vyžaduje 3 kroky:

- [Vytvorte politiku dodržiavania súladu a definujte nastavenia, ktoré je potrebné splniť pred tým, ako sa zariadenie považuje za vyhovujúce. Zariadenie musí mať napríklad PIN kód aspoň 6 číslic, kým sa považuje za vyhovujúce.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Vytvorenie politiky podmieneného prístupu, ktorá definuje, aké zdroje sú chránené, a aké podmienky je potrebné splniť na prístup k týmto zdrojom. Zariadenie musí byť napríklad kompatibilné pred prístupom k podnikovému e-mailu.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Zabezpečte, aby politiky dodržiavania súladu a politiky podmieneného prístupu boli zacielené na požadované skupiny používateľov. Môže to vyžadovať vytvorenie konkrétnych skupín používateľov v službe Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Ďalšie informácie...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
