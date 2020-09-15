---
title: 1554 Winsock error 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698877"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="2dac2-102">Chyba rozhrania Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="2dac2-102">Winsock error 10061</span></span>

<span data-ttu-id="2dac2-103">Tento kód chyby znamená, že spoločnosť Microsoft nedokáže vytvoriť zásuvku TCP (pripojenie) s cieľovým hostiteľom.</span><span class="sxs-lookup"><span data-stu-id="2dac2-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="2dac2-104">Najpravdepodobnejšou príčinou tejto chyby je problém s konfiguráciou brány firewall.</span><span class="sxs-lookup"><span data-stu-id="2dac2-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="2dac2-105">Ak chcete problém vyriešiť, skontrolujte tieto nastavenia:</span><span class="sxs-lookup"><span data-stu-id="2dac2-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="2dac2-106">Overenie konfigurácie brány firewall s informáciami v [rozsahu URL adries a rozsahov IP adries v Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="2dac2-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="2dac2-107">Ak je chyba špecifická pre Exchange Online Protection (EOP), mali by ste byť predtým upozornení na zmenu [IP adries ochrany v službe Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="2dac2-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="2dac2-108">Overte, či poskytovateľ internetových služieb (ISP) neblokuje port.</span><span class="sxs-lookup"><span data-stu-id="2dac2-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="2dac2-109">Overte nastavenia inteligentného hostiteľa a cieľového servera v konektoroch.</span><span class="sxs-lookup"><span data-stu-id="2dac2-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="2dac2-110">Všimnite si, že Microsoft 365 neblokuje *prichádzajúce* pripojenia týmto spôsobom.</span><span class="sxs-lookup"><span data-stu-id="2dac2-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
