---
title: Konfigurácia nastavení politiky Microsoft Edgeu vo Windowse
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
- "9004632"
- "6894"
- "8358"
ms.openlocfilehash: e9bb489b4d8ecd76fd777ade9fb740ecad542900
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402390"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="2fa7c-102">Konfigurácia nastavení politiky Microsoft Edgeu vo Windowse</span><span class="sxs-lookup"><span data-stu-id="2fa7c-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="2fa7c-103">Ak chcete konfigurovať nastavenia politiky a spravované aktualizácie pre Microsoft Edge, použite objekty skupinovej politiky (GPOS).</span><span class="sxs-lookup"><span data-stu-id="2fa7c-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="2fa7c-104">Politiku môžete poskytnúť aj prostredníctvom databázy Registry. toto by bolo vhodné pre (1) zariadenia s Windowsom pripojené k doméne Microsoft Active Directory a pre (2) inštancie Windowsu 10 Pro a Enterprise zaregistrované na správu zariadení v službe Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="2fa7c-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="2fa7c-105">Ak chcete Microsoft Edge nakonfigurovať pomocou procesorov GPO, vykonajte nasledovné:</span><span class="sxs-lookup"><span data-stu-id="2fa7c-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="2fa7c-106">Prejdite do centrálneho ukladacieho priestoru skupinovej politiky v doméne služby Active Directory alebo do priečinka šablóny Definícia politiky na jednotlivých počítačoch, nainštalujte všetky šablóny na správu, ktoré pridajú pravidlá a nastavenia pre Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="2fa7c-106">Go to the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="2fa7c-107">Nakonfigurujte konkrétne politiky, ktoré chcete nastaviť.</span><span class="sxs-lookup"><span data-stu-id="2fa7c-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="2fa7c-108">Ďalšie informácie nájdete v téme Konfigurácia [nastavení politiky Microsoft Edgeu vo Windowse.](https://go.microsoft.com/fwlink/?linkid=2135024)</span><span class="sxs-lookup"><span data-stu-id="2fa7c-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
