---
title: Podmienený prístup so službou Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704801"
---
# <a name="conditional-access-with-intune"></a>Podmienený prístup so službou Intune

Používanie  **podmieneného prístupu**  so službou Intune vyžaduje 3 kroky:

- Vytvorte  **politiku dodržiavania súladu**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) a definujte nastavenia, ktoré je potrebné splniť pred tým, ako sa zariadenie považuje za vyhovujúce. Zariadenie musí mať napríklad PIN kód aspoň 6 číslic, kým sa považuje za vyhovujúce.
- Vytvorenie **politiky podmieneného prístupu**  , ktorá definuje, aké zdroje sú chránené, a aké podmienky je potrebné splniť na prístup k týmto zdrojom.  Zariadenie musí byť [napríklad](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) kompatibilné pred prístupom k podnikovému e-mailu.
- Zabezpečte, aby **politiky dodržiavania súladu**  a  **politiky podmieneného prístupu**  boli zacielené na požadované skupiny používateľov. Môže to vyžadovať vytvorenie konkrétnych skupín používateľov v službe Azure Active Directory.

**Užitočné prepojenia:**

[Prehľad súladu zariadenia](https://docs.microsoft.com/intune/device-compliance-get-started)

[Riešenie problémov s certifikačnou autoritou](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Politika riešenia problémov](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Ak chcete zabezpečiť e-maily (Exchange Online) z Accessu v nevyhovujúcich zariadeniach, musia sa použiť obidva dokumenty:

1. [Ochrana e-mailového prístupu zo zariadení pomocou EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Ochrana e-mailového prístupu zo zariadení pomocou moderných klientov overovania, ako je Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)