---
title: Riešenie problémov s bezpečnostným tipom na kontrolu podvodov
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504998"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Riešenie problémov s bezpečnostným tipom na kontrolu podvodov

Ak dostávate bezpečnostný tip s textom "Odosielateľ zlyhal pri kontrole podvodov a nemusí byť tým, kým sa zdá byť", potom sa odosielateľovi nepodarilo prejsť kontrolou overovania DKIM alebo SPF. Najlepší spôsob, ako to vyriešiť, je pre odosielateľa, aby saautori sami. Ak odosielateľ odosiela vo vašom mene, musíte ich autorizovať pridaním adresy IP odosielateľa do záznamu SPF.
  
Ďalšie informácie nájdete v časti [Riešenie problémov s červeným (podozrivým) bezpečnostným tipom na kontrolu podvodov.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)
  
Tu je niekoľko ďalších odkazov, ktoré môžu pomôcť:
  
- [Ako spoločnosť Microsoft používa rámec politiky odosielateľa (SPF) na zabránenie falšovaniu](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Nastavenie protokolu SPF na zabránenie falšovaniu](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
