---
title: Riešenie problémov so zvukom vo Windowse 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750358"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="31402-102">Riešenie problémov so zvukom vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="31402-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="31402-103">**Spustenie Poradcu pri riešení problémov so zvukom**</span><span class="sxs-lookup"><span data-stu-id="31402-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="31402-104">Otvorte [nastavenia riešenia problémov](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="31402-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="31402-105">Vyberte položku **Prehrať zvuk**  >  **spustite Poradcu pri riešení problémov**.</span><span class="sxs-lookup"><span data-stu-id="31402-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="31402-106">**Nastavenie predvoleného zariadenia**</span><span class="sxs-lookup"><span data-stu-id="31402-106">**Set the default device**</span></span>

<span data-ttu-id="31402-107">Ak sa pripájate k zvukovému zariadeniu pomocou USB alebo HDMI, možno bude potrebné toto zariadenie nastaviť ako predvolené:</span><span class="sxs-lookup"><span data-stu-id="31402-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="31402-108">Otvorte položku **Spustiť**  >  **zvuk**a potom v zozname výsledkov vyberte možnosť **zvuk** alebo **zmeniť systémové zvuky** .</span><span class="sxs-lookup"><span data-stu-id="31402-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="31402-109">Na karte **Prehrať** vyberte zariadenie, vyberte položku **nastaviť predvolené**a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="31402-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="31402-110">**Kontrola káblov, hlasitosti, reproduktorov a slúchadiel**</span><span class="sxs-lookup"><span data-stu-id="31402-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="31402-111">Skontrolujte pripojenie reproduktorov a slúchadiel k uvoľneným káblom a skontrolujte, či sú pripojené k správnej zásuvke.</span><span class="sxs-lookup"><span data-stu-id="31402-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="31402-112">Skontrolujte úrovne výkonu a hlasitosti a skúste zapnúť všetky ovládacie prvky hlasitosti.</span><span class="sxs-lookup"><span data-stu-id="31402-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="31402-113">Niektoré reproduktory a aplikácie majú vlastné ovládacie prvky hlasitosti. možno budete musieť skontrolovať všetky, aby ste sa uistili, že sú na správnej úrovni.</span><span class="sxs-lookup"><span data-stu-id="31402-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="31402-114">Skúste sa pripojiť pomocou iného USB portu.</span><span class="sxs-lookup"><span data-stu-id="31402-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="31402-115">**Poznámka**: Nezabudnite, že reproduktory nemusia fungovať, keď sú zapojené slúchadlá.</span><span class="sxs-lookup"><span data-stu-id="31402-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="31402-116">**Kontrola správcu zariadení**</span><span class="sxs-lookup"><span data-stu-id="31402-116">**Check Device Manager**</span></span>

<span data-ttu-id="31402-117">Ak chcete skontrolovať, či sú ovládače aktuálne:</span><span class="sxs-lookup"><span data-stu-id="31402-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="31402-118">Vyberte položku **Štart**, zadajte výraz **Správca zariadení**a potom v zozname výsledkov vyberte položku **Správca zariadení** .</span><span class="sxs-lookup"><span data-stu-id="31402-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="31402-119">V časti **Ovládacie prvky zvuku, videa a hier**vyberte zvukovú kartu, otvorte ju, vyberte kartu **ovládač** a vyberte položku **aktualizovať ovládač**.</span><span class="sxs-lookup"><span data-stu-id="31402-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="31402-120">**Poznámka**: Ak Windows nenájde nový ovládač, vyhľadajte ho na webovej lokalite výrobcu zariadenia a postupujte podľa pokynov.</span><span class="sxs-lookup"><span data-stu-id="31402-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="31402-121">**Preinštalovanie ovládača**</span><span class="sxs-lookup"><span data-stu-id="31402-121">**Reinstall the driver**</span></span>

<span data-ttu-id="31402-122">Ak nie je možné aktualizovať prostredníctvom správcu zariadení alebo nájsť nový ovládač na webovej lokalite výrobcu, vyskúšajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="31402-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="31402-123">V Správcovi zariadení kliknite pravým tlačidlom myši na ovládač zvuku (alebo ho stlačte a podržte) a vyberte položku **odinštalovať**.</span><span class="sxs-lookup"><span data-stu-id="31402-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="31402-124">Reštartujte zariadenie a Windows sa pokúsi ovládač preinštalovať.</span><span class="sxs-lookup"><span data-stu-id="31402-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="31402-125">Ak opätovne nainštalujete ovládač, skúste použiť všeobecný zvukový ovládač, ktorý je súčasťou Windowsu.</span><span class="sxs-lookup"><span data-stu-id="31402-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="31402-126">V Správcovi zariadení kliknite pravým tlačidlom myši na ovládač zvuku (alebo ho stlačte a podržte) > **aktualizujte softvér ovládača**  >  **vyhľadajte v počítači softvér ovládača**  >  , ktorý**mi umožní vybrať zo zoznamu ovládačov zariadení v mojom počítači**, vyberte položku Ďalšie **zvukové zariadenie**, vyberte položku **ďalej**a postupujte podľa pokynov na jej inštaláciu.</span><span class="sxs-lookup"><span data-stu-id="31402-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
