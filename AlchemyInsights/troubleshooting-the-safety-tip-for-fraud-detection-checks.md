---
title: Riešenie problémov s bezpečnostným hrotom pre kontroly detekcie podvodov
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
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759527"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Riešenie problémov s bezpečnostným hrotom pre kontroly detekcie podvodov

Ak ste získali bezpečnostný tip, ktorý hovorí, že "odosielateľ zlyhal naše kontroly podvodov detekcie a nemusí byť, kto sa zdajú byť", potom odosielateľ zlyhal odovzdať buď DKIM alebo SPF overovanie kontroly. Najlepšia metóda na vyriešenie tohto problému je pre odosielateľa, ktorý sa má autorizovať. Ak odosielateľ odosiela váš účet, musíte ich autorizovať pridaním adresy IP odosielateľa do záznamu SPF.
  
Ďalšie informácie nájdete [v téme Riešenie problémov s červeným (podozrivým) bezpečnostným tipom na kontrolu podvodov](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Tu je niekoľko ďalších prepojení, ktoré môžu pomôcť:
  
- [Ako Microsoft používa odosielateľa politiky rámec (SPF) zabrániť falšovanie](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Nastavenie SPF na zabránenie falošnej spoofing](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
