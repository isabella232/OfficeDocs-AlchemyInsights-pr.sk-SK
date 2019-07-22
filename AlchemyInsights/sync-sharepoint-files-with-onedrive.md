---
title: Riešenie problémov s príkazom Otvoriť v programe Prieskumník v SharePointe Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 13149d288336b487441c66521b32406e408911fd
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/19/2019
ms.locfileid: "35803053"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="21ccc-102">Riešenie problémov s príkazom Otvoriť v programe Prieskumník v SharePointe Online</span><span class="sxs-lookup"><span data-stu-id="21ccc-102">Troubleshoot “Open with Explorer” issues in Sharepoint Online</span></span>

<span data-ttu-id="21ccc-103">Príkaz Otvoriť v programe Prieskumník otvorí lokálnu inštanciu Windows Prieskumníka, ktorá zobrazí štruktúru priečinkov na serveri hosťujúcom lokalitu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="21ccc-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="21ccc-104">Vzhľadom na to, čo bolo povedané, odporúčame [synchronizovať súbory SharePointu s novým synchronizačným klientom pre OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, ktorý poskytuje [súbory na požiadanie](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), pretože poskytuje lokálny prístup k vašim súborom a ponúka najlepší výkon.</span><span class="sxs-lookup"><span data-stu-id="21ccc-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="21ccc-105">Ak ste sa miesto nového synchronizačného klienta pre OneDrive rozhodli použiť zobrazenie v Prieskumníkovi, postupujte podľa krokov a najvhodnejších postupov v týchto článkoch:</span><span class="sxs-lookup"><span data-stu-id="21ccc-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="21ccc-106">Riešenie problémov v SharePointe Online pomocou príkazu Otvoriť v programe Prieskumník</span><span class="sxs-lookup"><span data-stu-id="21ccc-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="21ccc-107">Kopírovanie alebo premiestňovanie súborov v knižnici pomocou príkazu Otvoriť v programe Prieskumník</span><span class="sxs-lookup"><span data-stu-id="21ccc-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="21ccc-108">Tlačidlo **Otvoriť v programe Prieskumník** sa nezobrazuje v prostredí novej knižnice.</span><span class="sxs-lookup"><span data-stu-id="21ccc-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="21ccc-109">Vyberte rozbaľovaciu ponuku **Zobraziť** v pravom hornom rohu (názov rozbaľovacej ponuky závisí od aktuálneho zobrazenia) a potom vyberte položku **Zobraziť v Prieskumníkovi**.</span><span class="sxs-lookup"><span data-stu-id="21ccc-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

 ><span data-ttu-id="21ccc-110">Príkaz Otvoriť v programe Prieskumník v SharePointe používa ovládacie prvky ActiveX, takže je podporovaný iba v Internet Exploreri 10 alebo 11.</span><span class="sxs-lookup"><span data-stu-id="21ccc-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="21ccc-111">Príkaz Otvoriť v programe Prieskumník nefunguje vo Windowse s prehliadačmi Microsoft Edge, Google Chrome, Mozilla Firefox, ani na platforme Mac.</span><span class="sxs-lookup"><span data-stu-id="21ccc-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="21ccc-112">Z tohto dôvodu môžete mať možnosť Zobrazenie Prieskumníka neaktívnu.</span><span class="sxs-lookup"><span data-stu-id="21ccc-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

> - <span data-ttu-id="21ccc-113">[Príčiny nedostupnosti alebo neaktívnosti tlačidiel na páse s nástrojmi v SharePointe](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="21ccc-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

