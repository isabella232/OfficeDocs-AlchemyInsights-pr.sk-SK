---
title: Ovládanie automatických aktualizácií aplikácií balíka Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439924"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="1ebe3-102">Ovládanie automatických aktualizácií aplikácií balíka Office</span><span class="sxs-lookup"><span data-stu-id="1ebe3-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="1ebe3-103">V predvolenom nastavení sa aktualizácie aplikácií balíka Office preberajú automaticky a použijú na pozadí bez akéhokoľvek zásahu používateľa.</span><span class="sxs-lookup"><span data-stu-id="1ebe3-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="1ebe3-104">Správcovia však môžu ovládať spôsob, akým sa používajú aktualizácie pomocou nastavenia služby Office Update.</span><span class="sxs-lookup"><span data-stu-id="1ebe3-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="1ebe3-105">Nastavenia aktualizácie umožňujú správcom povoliť alebo zakázať automatické aktualizácie, zobraziť alebo skryť **tlačidlo Aktualizovať v** balíku Office, nastaviť termíny aktualizácií a ďalšie.</span><span class="sxs-lookup"><span data-stu-id="1ebe3-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="1ebe3-106">Podrobné informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="1ebe3-106">For detailed information, see:</span></span>

- [<span data-ttu-id="1ebe3-107">Konfigurácia nastavenia aktualizácie balíka Office</span><span class="sxs-lookup"><span data-stu-id="1ebe3-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="1ebe3-108">Automatické aktualizácie balíka Office nie je povolená</span><span class="sxs-lookup"><span data-stu-id="1ebe3-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="1ebe3-109">Definovanie spôsobu aktualizácie balíka Office po jeho nainštalovaní</span><span class="sxs-lookup"><span data-stu-id="1ebe3-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="1ebe3-110">Ak chcete skontrolovať existujúce nastavenia aktualizácií použité na klientskom počítači, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="1ebe3-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="1ebe3-111">Otvorte Editor databázy Registry tým, že **pôjdete**  >  **na Štart Spustiť**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="1ebe3-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="1ebe3-112">Prepnite sa do nasledujúceho umiestnenia a skontrolujte nastavenia služby Office Update:</span><span class="sxs-lookup"><span data-stu-id="1ebe3-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="1ebe3-113">a.</span><span class="sxs-lookup"><span data-stu-id="1ebe3-113">a.</span></span> <span data-ttu-id="1ebe3-114">HKEY_LOCAL_MACHINE SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="1ebe3-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="1ebe3-115">b.</span><span class="sxs-lookup"><span data-stu-id="1ebe3-115">b.</span></span> <span data-ttu-id="1ebe3-116">Kliknite na tlačidloToRun\Konfigurácia</span><span class="sxs-lookup"><span data-stu-id="1ebe3-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="1ebe3-117">**Upozornenie:**  Ak je nastavený kľúč OfficeMgmtCOM, môže sa zobraziť hlásenie "Aktualizácie spravuje správca systému" v **aktualizáciách balíka Office**  >  **Account**  >  **Account Office**.</span><span class="sxs-lookup"><span data-stu-id="1ebe3-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="1ebe3-118">Ďalšie informácie nájdete v téme [Správa aktualizácií aplikácií Microsoft 365 pomocou programu Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="1ebe3-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  