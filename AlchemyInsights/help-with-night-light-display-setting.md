---
title: Pomoc s nastavením nočného osvetlenia
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405180"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="9c956-102">Pomoc s nastavením nočného osvetlenia</span><span class="sxs-lookup"><span data-stu-id="9c956-102">Help with the night light display setting</span></span>

<span data-ttu-id="9c956-103">Ďalšie informácie o nastaveniach nočného času zobrazenia nájdete v [téme Nastavenie nočného času obrazovky vo Windowse 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="9c956-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="9c956-104">Ak sú možnosti nočného osvetlenia v nastaveniach sivé, skontrolujte ovládač obrazovky:</span><span class="sxs-lookup"><span data-stu-id="9c956-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="9c956-105">Kliknite na vyhľadávacie pole na paneli úloh a zadajte výraz **Správca** zariadení a potom vo **výsledkoch hľadania** vyberte položku Správca zariadení.</span><span class="sxs-lookup"><span data-stu-id="9c956-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="9c956-106">Rozbaľte **položku Display adapters (Zobrazovacie adaptéry).**</span><span class="sxs-lookup"><span data-stu-id="9c956-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="9c956-107">Funkcia nočného osvetlenia však nie je k dispozícii, ak vaše zariadenie používa ovládač DisplayLink alebo ovládač základného zobrazenia.</span><span class="sxs-lookup"><span data-stu-id="9c956-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="9c956-108">Funkcia nočného osvetlenia využíva najnovšie grafické technológie, preto môže byť potrebné aktualizovať ovládač obrazovky:</span><span class="sxs-lookup"><span data-stu-id="9c956-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="9c956-109">Ak chcete vyhľadať aktualizácie, vyberte **položky**  >  **Nastavenie aktualizácie**&  >  **Zabezpečenie** Služby Windows  >  **Update**  >  **Vyhľadať aktualizácie.**</span><span class="sxs-lookup"><span data-stu-id="9c956-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="9c956-110">ALEBO</span><span class="sxs-lookup"><span data-stu-id="9c956-110">OR</span></span>

- <span data-ttu-id="9c956-111">Ak chcete manuálne stiahnuť a nainštalovať najnovšie ovládače obrazovky, navštívte webovú lokalitu podpory výrobcu hardvéru.</span><span class="sxs-lookup"><span data-stu-id="9c956-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="9c956-112">Resetovanie nočného osvetlenia v databáze Registry</span><span class="sxs-lookup"><span data-stu-id="9c956-112">Reset night light in the registry</span></span>

<span data-ttu-id="9c956-113">Ak aktualizácia ovládača obrazovky nefunguje, možno bude v databáze Registry potrebné obnoviť nočné osvetlenie.</span><span class="sxs-lookup"><span data-stu-id="9c956-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="9c956-114">**Upozornenie:** Tento krok riešenia problémov sa odporúča iba pre pokročilých používateľov.</span><span class="sxs-lookup"><span data-stu-id="9c956-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="9c956-115">Ak databázu Registry upravíte nesprávne, môžu sa vyskytnúť závažné problémy.</span><span class="sxs-lookup"><span data-stu-id="9c956-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="9c956-116">Na ešte pridanú ochranu si databázu Registry pred úpravou zálohujte, aby ste ju v prípade problémov mohli obnoviť.</span><span class="sxs-lookup"><span data-stu-id="9c956-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="9c956-117">Do vyhľadávacieho poľa zadajte príkaz **regedit** a potom vo výsledkoch hľadania vyberte položku **Editor** databázy Registry.</span><span class="sxs-lookup"><span data-stu-id="9c956-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="9c956-118">Prejdite na nasledujúci kľúč databázy Registry:</span><span class="sxs-lookup"><span data-stu-id="9c956-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="9c956-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="9c956-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="9c956-120">Export a potom odstráňte nasledujúci podkľúč:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="9c956-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="9c956-121">Export a potom odstráňte nasledujúci podkľúč:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="9c956-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="9c956-122">Reštartujte Windows a overte, či sú k dispozícii možnosti nočného osvetlenia.</span><span class="sxs-lookup"><span data-stu-id="9c956-122">Restart Windows and verify if the night light options are available.</span></span>


