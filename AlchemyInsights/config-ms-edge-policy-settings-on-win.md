---
title: Konfigurácia nastavení politiky Microsoft Edge vo Windowse
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583744"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="51266-102">Konfigurácia nastavení politiky Microsoft Edge vo Windowse</span><span class="sxs-lookup"><span data-stu-id="51266-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="51266-103">Ak chcete konfigurovať nastavenie politiky a spravované aktualizácie pre Microsoft Edge, použite objekty skupinovej politiky (GPO).</span><span class="sxs-lookup"><span data-stu-id="51266-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="51266-104">Môžete tiež poskytnúť politiku prostredníctvom databázy Registry. bolo by vhodné, aby sa zariadenia s Windowsom (1) pripojili k doméne služby Microsoft Active Directory a pre (2) Windows 10 Pro a Enterprise inštancie zapísali pre správu zariadenia v službe Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="51266-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="51266-105">Ak chcete nakonfigurovať Microsoft Edge pomocou GPOs, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="51266-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="51266-106">Do centrálneho ukladacieho priestoru skupinovej politiky v doméne služby Active Directory alebo do priečinka šablóny definícií politiky v jednotlivých počítačoch nainštalujte všetky šablóny na správu, ktoré pridávajú pravidlá a nastavenia pre Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="51266-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="51266-107">Nakonfigurujte konkrétne politiky, ktoré chcete nastaviť.</span><span class="sxs-lookup"><span data-stu-id="51266-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="51266-108">Ďalšie informácie nájdete v téme [Konfigurácia nastavení politiky Microsoft Edge vo Windowse](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="51266-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
