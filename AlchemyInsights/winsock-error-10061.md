---
title: 1554 chyba rozhrania Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766184"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="bbaf4-102">Chyba rozhrania Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="bbaf4-102">Winsock error 10061</span></span>

<span data-ttu-id="bbaf4-103">Tento kód chyby znamená, že spoločnosť Microsoft nemohla vytvoriť soket TCP (pripojenie) s cieľovým hostiteľom.</span><span class="sxs-lookup"><span data-stu-id="bbaf4-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="bbaf4-104">Najpravdepodobnejšou príčinou tejto chyby je problém s konfiguráciou brány firewall.</span><span class="sxs-lookup"><span data-stu-id="bbaf4-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="bbaf4-105">Ak chcete problém vyriešiť, skontrolujte tieto nastavenia:</span><span class="sxs-lookup"><span data-stu-id="bbaf4-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="bbaf4-106">Overte konfiguráciu brány firewall s informáciami v [Microsoft 365 URL a rozsahy adries IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="bbaf4-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="bbaf4-107">Ak je chyba špecifická pre Exchange Online Protection (EOP), mali by ste boli predtým upozornení na zmenu [Exchange Online Protection IP adresy](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="bbaf4-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="bbaf4-108">Overte, či poskytovateľ internetových služieb (ISP) neblokuje port.</span><span class="sxs-lookup"><span data-stu-id="bbaf4-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="bbaf4-109">Skontrolujte nastavenia inteligentných hostiteľov a cieľového servera v konektoroch.</span><span class="sxs-lookup"><span data-stu-id="bbaf4-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="bbaf4-110">Všimnite si, že Microsoft 365 neblokuje *prichádzajúce* pripojenia týmto spôsobom.</span><span class="sxs-lookup"><span data-stu-id="bbaf4-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
