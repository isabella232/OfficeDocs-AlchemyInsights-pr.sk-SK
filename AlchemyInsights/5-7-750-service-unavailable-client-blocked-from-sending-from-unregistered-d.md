---
title: Služba 5.7.750 služby 1048 nie je k dispozícii. Klient zablokoval odosielanie z neregistrovaných domén
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664257"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="e88af-103">5.7.750 klient zablokoval odoslanie z neregistrovanej domény</span><span class="sxs-lookup"><span data-stu-id="e88af-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="e88af-104">Chyba sa vyskytuje pri odoslaní veľkého objemu správ z domén, ktoré nie sú v nájomníkovi uvedené (pridané ako akceptované domény a overené).</span><span class="sxs-lookup"><span data-stu-id="e88af-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="e88af-105">Ak sa chcete vyhnúť tejto chybe, môžete použiť spojnicu toku pošty na základe certifikátu, kde je doménou certifikátu poskytnutá doména, alebo môžete ustanoviť všetky odosielajúce domény.</span><span class="sxs-lookup"><span data-stu-id="e88af-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
