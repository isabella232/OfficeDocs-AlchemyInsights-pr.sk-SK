---
title: 1049 AntiSpam 4.5.3 príliš veľa príjemcov (AS780090)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1049"
- "3100024"
ms.assetid: fa3d4be9-c90a-4926-9754-4b708b038bf6
ms.openlocfilehash: deb57e6e872ce5769a339c7d130a63a8e90ab4c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717808"
---
# <a name="453-too-many-recipients-as780090"></a><span data-ttu-id="d09a4-102">4.5.3 príliš veľa príjemcov (AS780090)</span><span class="sxs-lookup"><span data-stu-id="d09a4-102">4.5.3 Too many recipients (AS780090)</span></span>

<span data-ttu-id="d09a4-103">Táto chyba sa vyskytuje vtedy, keď je objem e-mailovej prenosnosti zo zdrojovej IP adresy väčší ako limit na základe dobrého mena (alebo nedostatočnej reputácie) zdrojovej IP adresy.</span><span class="sxs-lookup"><span data-stu-id="d09a4-103">This error occurs when the volume of email traffic from the source IP address exceeds the limit based on the reputation (or lack of reputation) of source IP address.</span></span>

<span data-ttu-id="d09a4-104">Zablokovanie e-mailu zo zdrojovej IP adresy sa skončí v priebehu hodiny.</span><span class="sxs-lookup"><span data-stu-id="d09a4-104">Blocking email from the source IP address will expire within an hour.</span></span> <span data-ttu-id="d09a4-105">Ak je zdrojovou IP adresou lokálny e-mailový server, ktorý patrí vám, overte konfiguráciu konektora toku pošty.</span><span class="sxs-lookup"><span data-stu-id="d09a4-105">If the source IP address is an on-premises email server that belongs to you, verify the configuration of the mail flow connector.</span></span> <span data-ttu-id="d09a4-106">Ak správanie trvá dlhšie ako hodinu, obráťte sa na oddelenie podpory a požiadajte o výnimku pre zdrojovú IP adresu.</span><span class="sxs-lookup"><span data-stu-id="d09a4-106">If the behavior continues for more than an hour, contact support to request an exception for the source IP address.</span></span>
