---
title: Povolenie programu Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive a Microsoft teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747741"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="3b76e-102">Povolenie programu Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive a Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="3b76e-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="3b76e-103">Pomocou poverení globálneho správcu alebo správcu zabezpečenia sa prihláste do [Centra zabezpečenia a dodržiavania súladu pre Office 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="3b76e-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="3b76e-104">Na ľavej table vyberte položku **Správa hrozieb** a potom vyberte položku   >  [bezpečnostné prílohy](https://protection.office.com/safeattachment)politiky.</span><span class="sxs-lookup"><span data-stu-id="3b76e-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="3b76e-105">Vyberte položku **Zapnúť Microsoft Defender pre Office 365 pre SharePoint, OneDrive a Microsoft teams** a potom vyberte položku **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="3b76e-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="3b76e-106">Ako globálny správca alebo správca SharePointu Online spustite nasledujúcu rutinu typu cmdlet prostredia PowerShell s parametrom **DisallowInfectedFileDownload** nastaveným na *hodnotu True*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="3b76e-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="3b76e-107">Nastavenie upozornení na zistené súbory</span><span class="sxs-lookup"><span data-stu-id="3b76e-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="3b76e-108">Ďalšie informácie nájdete v téme [Microsoft Defender pre Office 365 pre SharePoint, OneDrive a Microsoft teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span><span class="sxs-lookup"><span data-stu-id="3b76e-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
