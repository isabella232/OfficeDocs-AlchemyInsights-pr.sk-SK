---
title: Riešenie problémov s zapísať zariadenia so systémom Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559676"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Riešenie problémov s zapísať zariadenia so systémom Windows Microsoft Intune

Preskúmanie zdrojov uvedených nižšie vyriešiť váš problém teraz.
  
Niektoré bežné chybové hlásenia a rozlíšenie kroky:
  
 **Nemôže byť nainštalovaný softvér, 0x80cf4017:** Váš účet certifikátu skončila. Re-Stiahnuť softvérový balík PC klienta v Intune Admin konzole. Ďalšie informácie v tejto dokumentácii.
  
 **Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledovných prípadoch:
  
1. Užívateľ má viac zariadení zaradených ako limit zariadenia. Revidovať tieto dokumenty [Odstránenie zariadenia](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeniť limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

2. "Používatelia môžu pripojiť zariadenia Azure AD" je nastavený na "none". Nastavte ju na všetky, alebo vybrať používateľov. Prečítajte si [túto dokumentáciu](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) ďalšie informácie.

3. Zariadenie je už zaregistrovaná iným používateľom. Ak je to prípad, odstrániť zariadenie z Azure Intune konzoly alebo manuálne unenroll zariadenie pred opätovným pokusom.

4. Zariadenie je Windows 10 Home. Iba Windows 10 Pro, vzdelávanie a Enterprise SKU môžete pripojiť Azure služby Active Directory.

Dodatočné zdroje, ktoré pomôžu vyriešiť váš problém:
  
1. Používajte [Windows Intune riešenia problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhania registrácie. Prečítať [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre ďalšie podrobnosti.

2. Revidovať tieto dokumenty zoznam bežných chýb, ktoré bránia zápisnice a uznesenia každému: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [Riešenie problémov doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Naučte sa zapísať zariadenia so systémom Windows v spoločnosti Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
