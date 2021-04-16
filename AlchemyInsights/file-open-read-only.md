---
title: Súbor otvorený iba na čítanie
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813199"
---
# <a name="file-open-read-only"></a><span data-ttu-id="7844d-102">Súbor otvorený iba na čítanie</span><span class="sxs-lookup"><span data-stu-id="7844d-102">File open read-only</span></span>

<span data-ttu-id="7844d-103">Možno zistíte, že keď otvárate súbory, otvoria sa iba na čítanie.</span><span class="sxs-lookup"><span data-stu-id="7844d-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="7844d-104">V niektorých prípadoch je to z dôvodu pridanej bezpečnosti, napríklad pri otváraní súborov z internetu, a inokedy to môže byť z dôvodu nastavenia, ktoré je možné zmeniť.</span><span class="sxs-lookup"><span data-stu-id="7844d-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="7844d-105">Tu sú niektoré scenáre, keď sa súbor otvorí iba na čítanie, a niekoľko krokov, ktoré môžete vykonať, ak to chcete zmeniť.</span><span class="sxs-lookup"><span data-stu-id="7844d-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="7844d-106">**Môj antivírusový program spôsobuje, že sa otvárajú iba na čítanie**</span><span class="sxs-lookup"><span data-stu-id="7844d-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="7844d-107">Niektoré antivírusové programy vás môžu chrániť pred potenciálne nebezpečnými súbormi ich otvorením iba na čítanie.</span><span class="sxs-lookup"><span data-stu-id="7844d-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="7844d-108">Informácie o úprave týchto nastavení vám možno bude potrebné skontrolovať u svojho poskytovateľa antivírusového programu.</span><span class="sxs-lookup"><span data-stu-id="7844d-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="7844d-109">Napríklad BitDefender obsahuje obsah na pridanie vylúčenia aplikácií tu: Pridanie vylúčenia aplikácií alebo procesov v ovládacom centre programu [Bitdefender.](https://aka.ms/AA6098i)</span><span class="sxs-lookup"><span data-stu-id="7844d-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="7844d-110">**Sú vlastnosti súboru nastavené iba na čítanie?**</span><span class="sxs-lookup"><span data-stu-id="7844d-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="7844d-111">Vlastnosti súboru môžete skontrolovať kliknutím pravým tlačidlom myši na súbor a výberom položky Vlastnosti.</span><span class="sxs-lookup"><span data-stu-id="7844d-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="7844d-112">Ak je začiarknuté políčko atribútu iba na čítanie, zrušte jeho začiarknutie a kliknite na tlačidlo OK.</span><span class="sxs-lookup"><span data-stu-id="7844d-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="7844d-113">**Obsah je v chránenom zobrazení**</span><span class="sxs-lookup"><span data-stu-id="7844d-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="7844d-114">Súbory z internetu a z iných potenciálne nebezpečných umiestnení môžu obsahovať vírusy, červy a iné druhy malvéru, ktorý môže poškodiť počítač.</span><span class="sxs-lookup"><span data-stu-id="7844d-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="7844d-115">Toto je tiež bežné v prípade príloh e-mailov alebo stiahnutých súborov.</span><span class="sxs-lookup"><span data-stu-id="7844d-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="7844d-116">Na ochranu počítača sa súbory z potenciálne nebezpečných umiestnení otvárajú v chránenom zobrazení.</span><span class="sxs-lookup"><span data-stu-id="7844d-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="7844d-117">Pomocou chráneného zobrazenia môžete čítať súbor, prezerať si jeho obsah a zároveň znižovať riziká.</span><span class="sxs-lookup"><span data-stu-id="7844d-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="7844d-118">Ďalšie informácie o chránenom zobrazení a o tom, ako zmeniť nastavenia, nájdete v tomto článku: [Čo je chránené zobrazenie?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="7844d-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="7844d-119">**Je OneDrive plný?**</span><span class="sxs-lookup"><span data-stu-id="7844d-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="7844d-120">Ak je súbor uložený vo OneDrive a ukladací priestor vo OneDrive je plný, dokument bude možné uložiť, až keď budete v rámci svojho prideleného priestoru.</span><span class="sxs-lookup"><span data-stu-id="7844d-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="7844d-121">Svoje voľné miesto vo OneDrive môžete skontrolovať kliknutím na ikonu OneDrive v centre oznámení a výberom položky Spravovať ukladací priestor alebo môžete prejsť na položku , prihlásiť sa a zaznamenať množstvo používaného miesta v ľavej dolnej časti [https://onedrive.live.com](https://onedrive.live.com) obrazovky.</span><span class="sxs-lookup"><span data-stu-id="7844d-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="7844d-122">**Je balík Office aktivovaný?**</span><span class="sxs-lookup"><span data-stu-id="7844d-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="7844d-123">Ak sa Office neaktivuje alebo platnosť vášho predplatného uplynula, môžete byť v režime iba na čítanie s obmedzenou funkčnosťou.</span><span class="sxs-lookup"><span data-stu-id="7844d-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="7844d-124">Informácie o aktivácii balíka Office nájdete v téme: [Chyba produktu bez licencie a chyba aktivácie v Office.](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="7844d-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="7844d-125">**Ak všetko ostatné zlyhá...**</span><span class="sxs-lookup"><span data-stu-id="7844d-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="7844d-126">Skúste reštartovať počítač.</span><span class="sxs-lookup"><span data-stu-id="7844d-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="7844d-127">Inštalácia aktualizácií balíka Office</span><span class="sxs-lookup"><span data-stu-id="7844d-127">Install Office updates</span></span>
    
- <span data-ttu-id="7844d-128">Vykonanie online opravy balíka Office</span><span class="sxs-lookup"><span data-stu-id="7844d-128">Perform an Online repair of Office</span></span>
    

