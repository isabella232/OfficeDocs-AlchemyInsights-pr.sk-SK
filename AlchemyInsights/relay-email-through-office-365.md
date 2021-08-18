---
title: Prenos e-mailov prostredníctvom služieb Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 8f8b0780ebec2911b6698deee25e0fabe83bd9afef5fb3a6ef4c51cccd67fc7c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898563"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Nastavenie multifunkčného zariadenia alebo aplikácie na odosielanie e-mailov

Ak chcete získať informácie o možnostiach a postupoch, pozrite si tému [Nastavenie multifunkčného zariadenia alebo aplikácie na odosielanie e-mailov pomocou služieb Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Ak máte zariadenie alebo aplikáciu, ktorá nedávno prestala fungovať, najbežnejšie problémy sú:

- **Chyby týkajúce sa overovania pri používaní odosielania klienta SMTP Auth** Nedávno sme vykonali niekoľko zmien týkajúcich sa spôsobu overovania SMTP. Ďalšie informácie o riešení problémov nájdete v časti Neúspešné overovanie v téme Riešenie problémov s tlačiarňami, skenermi a [aplikáciami LOB,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)ktoré odosielali e-maily Microsoft 365 alebo Office 365.
- Pri zabezpečenom pripojení k serveru Office 365 prijmeme len **verziu TLS 1.2 Office 365** Ak používate zabezpečené pripojenie (TLS), uistite sa, že vaše aplikačné zariadenie podporuje TLS 1.2. Ďalšie informácie nájdete v téme [Príprava na TLS 1.2 v téme Office 365 a Office 365 GCC.](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)
 
Ďalšie problémy a riešenia nájdete v téme Riešenie problémov s tlačiarňami, skenermi a [aplikáciami LOB,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)ktoré odosielali e-maily pomocou Microsoft 365 alebo Office 365.

Ak chcete zobraziť ovplyvnené zariadenia, prejdite na [zostavu klienta overovania protokolu SMTP](https://protection.office.com/mailflow/dashboard).

**Poznámka:** Exchange Online sa nevyhodí scenárom hromadnej korešpondencie. Ak chcete odosielať hromadné komerčné e-maily (napríklad zákaznícke bulletiny), mali by ste použiť poskytovateľov tretích strán, ktorí sa v týchto službách špecializovaní na ne zídu.
