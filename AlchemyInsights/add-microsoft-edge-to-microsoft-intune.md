---
title: Pridanie prehliadača Microsoft Edge do služby Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194575"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="39dc5-102">Pridanie prehliadača Microsoft Edge do služby Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="39dc5-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="39dc5-103">Ak chcete mať možnosť nasadiť, konfigurovať, monitorovať a chrániť Microsoft Edge pre Windows 10, musíte ju najprv pridať do služby Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="39dc5-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="39dc5-104">Intune podporuje Microsoft Edge 77 a novšie verzie.</span><span class="sxs-lookup"><span data-stu-id="39dc5-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="39dc5-105">Intune zistí všetky už existujúce inštalácie prehliadača Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="39dc5-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="39dc5-106">Ak je Microsoft Edge nainštalovaný v používateľskom kontexte, Inštalácia systému prepíše inštaláciu v používateľskom kontexte.</span><span class="sxs-lookup"><span data-stu-id="39dc5-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="39dc5-107">Ak je Microsoft Edge nainštalovaný v kontexte systému, bude sa zaznamenávať úspešnosť inštalácie.</span><span class="sxs-lookup"><span data-stu-id="39dc5-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="39dc5-108">Vopred nainštalovaná verzia Microsoft Edge 77 a novšie verzie pre všetky kanály v používateľskom kontexte sa prepíšu v prehliadači Microsoft Edge nainštalovaným v kontexte systému.</span><span class="sxs-lookup"><span data-stu-id="39dc5-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="39dc5-109">**Základné**</span><span class="sxs-lookup"><span data-stu-id="39dc5-109">**Prerequisite**</span></span>

<span data-ttu-id="39dc5-110">Windows 10, verzia 1709 alebo novšia verzia</span><span class="sxs-lookup"><span data-stu-id="39dc5-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="39dc5-111">**Postup na pridanie hrany do služby Intune**</span><span class="sxs-lookup"><span data-stu-id="39dc5-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="39dc5-112">[Nakonfigurujte aplikáciu v službe Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="39dc5-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="39dc5-113">[Nakonfigurujte informácie o aplikácii](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="39dc5-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="39dc5-114">[Konfigurácia nastavení aplikácie](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="39dc5-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="39dc5-115">[Vyberte značky rozsahu (voliteľné)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="39dc5-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="39dc5-116">[Pridajte aplikáciu](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="39dc5-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="39dc5-117">Ak potrebujete ďalšiu pomoc, pozrite si tému [Riešenie problémov](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="39dc5-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




