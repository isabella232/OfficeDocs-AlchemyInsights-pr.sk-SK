---
title: Duplicitný záznam zariadenia na portáli
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
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814531"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="94bcc-102">Duplicitný záznam zariadenia na portáli</span><span class="sxs-lookup"><span data-stu-id="94bcc-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="94bcc-103">V prípade, že zariadenie lokalite Správcu konfigurácie správne nenahlási stav spoločnej správy, na portáli sa môžu pre zariadenie zobraziť 2 záznamy.</span><span class="sxs-lookup"><span data-stu-id="94bcc-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="94bcc-104">Ak chcete skontrolovať stav spoločnej správy, skontrolujte stĺpec **Spoločná správa** zariadenia v konzole Správcu konfigurácie.</span><span class="sxs-lookup"><span data-stu-id="94bcc-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="94bcc-105">Ak sa stĺpec nezobrazuje, môžete ho pridať kliknutím pravým tlačidlom myši na ľubovoľnú hlavičku stĺpca a jeho výberom zo zoznamu.</span><span class="sxs-lookup"><span data-stu-id="94bcc-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="94bcc-106">Hodnota Spoločná správa musí byť **Áno**.</span><span class="sxs-lookup"><span data-stu-id="94bcc-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="94bcc-107">Ak je hodnota **Nie**, v klientskom zariadení otvorte aplet klienta Správca konfigurácie a na karte Všeobecné začiarknite políčko **Spoločná správa**.</span><span class="sxs-lookup"><span data-stu-id="94bcc-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="94bcc-108">Ak je hodnota **Povolené**, označuje to problémy s komunikáciou klienta s bodom správy.</span><span class="sxs-lookup"><span data-stu-id="94bcc-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="94bcc-109">Skontrolujte súbor **CcmMessaging.log** v zariadení a preskúmajte možné problémy s pripojením.</span><span class="sxs-lookup"><span data-stu-id="94bcc-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="94bcc-110">Ak je hodnota **Vypnuté** a zariadenie je zapísané v službe Intune, uistite sa, že zariadenie prijalo politiku spoločnej správy kontrolou súboru **CoManagementHandler.log** v zariadení.</span><span class="sxs-lookup"><span data-stu-id="94bcc-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
