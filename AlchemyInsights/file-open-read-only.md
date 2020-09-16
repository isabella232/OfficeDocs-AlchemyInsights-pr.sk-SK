---
title: Súbor je otvorený iba na čítanie
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745622"
---
# <a name="file-open-read-only"></a><span data-ttu-id="03a6c-102">Súbor je otvorený iba na čítanie</span><span class="sxs-lookup"><span data-stu-id="03a6c-102">File open read-only</span></span>

<span data-ttu-id="03a6c-103">Možno zistíte, že pri otváraní súborov sa otvoria iba na čítanie.</span><span class="sxs-lookup"><span data-stu-id="03a6c-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="03a6c-104">V niektorých prípadoch ide o zvýšenie zabezpečenia, napríklad pri otváraní súborov z internetu a iných časoch môže to byť spôsobené nastavením, ktoré je možné zmeniť.</span><span class="sxs-lookup"><span data-stu-id="03a6c-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="03a6c-105">Tu je niekoľko scenárov, v ktorých sa súbor otvorí iba na čítanie, a v niektorých krokoch môžete vykonať zmenu.</span><span class="sxs-lookup"><span data-stu-id="03a6c-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="03a6c-106">**Môj antivírusový program spôsobuje otváranie iba na čítanie**</span><span class="sxs-lookup"><span data-stu-id="03a6c-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="03a6c-107">Niektoré antivírusové programy vám môžu zabezpečiť ochranu pred potenciálne nebezpečnými súbormi ich otvorením iba na čítanie.</span><span class="sxs-lookup"><span data-stu-id="03a6c-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="03a6c-108">Ak chcete zistiť, ako tieto nastavenia prispôsobiť, možno budete musieť overiť u svojho poskytovateľa antivírusového programu.</span><span class="sxs-lookup"><span data-stu-id="03a6c-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="03a6c-109">BitDefender, napríklad, má obsah na pridanie vylúčenia z aplikácií tu: [ako pridať vylúčenie aplikácií alebo procesov v centre BitDefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="03a6c-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="03a6c-110">**Sú vlastnosti súboru nastavené iba na čítanie?**</span><span class="sxs-lookup"><span data-stu-id="03a6c-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="03a6c-111">Vlastnosti súboru môžete skontrolovať kliknutím pravým tlačidlom myši na súbor a výberom položky Vlastnosti.</span><span class="sxs-lookup"><span data-stu-id="03a6c-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="03a6c-112">Ak je začiarknutý atribút iba na čítanie, môžete ho zrušiť a kliknúť na tlačidlo OK.</span><span class="sxs-lookup"><span data-stu-id="03a6c-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="03a6c-113">**Obsah je v chránenom zobrazení**</span><span class="sxs-lookup"><span data-stu-id="03a6c-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="03a6c-114">Súbory z internetu a z iných potenciálne nebezpečných umiestnení môžu obsahovať vírusy, červy alebo iné druhy malvéru, ktoré môžu poškodiť váš počítač.</span><span class="sxs-lookup"><span data-stu-id="03a6c-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="03a6c-115">Toto je tiež bežne v prípade e-mailových príloh alebo súborov, ktoré ste si stiahli.</span><span class="sxs-lookup"><span data-stu-id="03a6c-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="03a6c-116">Na zabezpečenie počítača sa súbory z týchto potenciálne nebezpečných umiestnení otvárajú v chránenom zobrazení.</span><span class="sxs-lookup"><span data-stu-id="03a6c-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="03a6c-117">Pomocou chráneného zobrazenia si môžete prečítať súbor a zobraziť jeho obsah pri znižovaní rizík.</span><span class="sxs-lookup"><span data-stu-id="03a6c-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="03a6c-118">Ďalšie informácie o chránenom zobrazení a zmene nastavení nájdete v tomto článku: [čo je chránené zobrazenie?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="03a6c-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="03a6c-119">**Je OneDrive plný?**</span><span class="sxs-lookup"><span data-stu-id="03a6c-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="03a6c-120">Ak je súbor uložený vo OneDrive a ukladací priestor vo OneDrive je plný, dokument nebude možné uložiť, kým nebudete v rámci prideleného priestoru.</span><span class="sxs-lookup"><span data-stu-id="03a6c-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="03a6c-121">Ak chcete skontrolovať voľné miesto vo OneDrive, kliknite na ikonu OneDrive v centre oznámení a vyberte položku Spravovať ukladací priestor alebo môžete prejsť na [https://onedrive.live.com](https://onedrive.live.com) , prihlásiť sa a poznačte si množstvo použitého miesta v ľavej dolnej časti obrazovky.</span><span class="sxs-lookup"><span data-stu-id="03a6c-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="03a6c-122">**Je Office aktivovaný?**</span><span class="sxs-lookup"><span data-stu-id="03a6c-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="03a6c-123">Ak sa balík Office neaktivuje alebo uplynula platnosť vášho predplatného, môže to byť v režime obmedzenej funkčnosti iba na čítanie.</span><span class="sxs-lookup"><span data-stu-id="03a6c-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="03a6c-124">Ďalšie informácie o aktivácii balíka Office nájdete v téme: chyby produktu bez platnej [licencie a chyby aktivácie v Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="03a6c-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="03a6c-125">**Ak všetko ostatné zlyhá...**</span><span class="sxs-lookup"><span data-stu-id="03a6c-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="03a6c-126">Skúste reštartovať počítač</span><span class="sxs-lookup"><span data-stu-id="03a6c-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="03a6c-127">Inštalácia aktualizácií balíka Office</span><span class="sxs-lookup"><span data-stu-id="03a6c-127">Install Office updates</span></span>
    
- <span data-ttu-id="03a6c-128">Vykonanie online opravy balíka Office</span><span class="sxs-lookup"><span data-stu-id="03a6c-128">Perform an Online repair of Office</span></span>
    

