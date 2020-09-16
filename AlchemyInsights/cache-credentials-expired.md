---
title: 'Chyba: zmeny sa nedajú nahrať ani stiahnuť, pretože platnosť poverení vo vyrovnávacej pamäti uplynula'
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 8105fa7b311bc932f95c8bff4d6b58ed9aabe74a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734494"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a><span data-ttu-id="cff77-102">Chyba: zmeny sa nedajú nahrať ani stiahnuť, pretože platnosť poverení vo vyrovnávacej pamäti uplynula</span><span class="sxs-lookup"><span data-stu-id="cff77-102">Error: We can't upload or download your changes because your cached credentials have expired</span></span>

<span data-ttu-id="cff77-103">Pri ukladaní súborov do aplikácie OneDrive, ak sa zobrazí chyba, ktorá obsahuje slovné spojenie **"vaše poverenia s vyrovnávacou pamäťou uplynuli"**, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="cff77-103">When saving files to the OneDrive app, if you receive an error that contains the phrase **"your cached credentials have expired"**, perform the following steps:</span></span>

1. <span data-ttu-id="cff77-104">Ukončite všetky aplikácie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="cff77-104">Close all Office applications.</span></span>
1. <span data-ttu-id="cff77-105">Otvorte Správcu poverení a do vyhľadávacieho poľa na paneli úloh zadajte výraz **Správca poverení** a potom vyberte položku **Ovládací panel Správca poverení**.</span><span class="sxs-lookup"><span data-stu-id="cff77-105">Open Credential Manager, and type **credential manager** in the search box on the taskbar, then select **Credential Manager Control panel**.</span></span>
1. <span data-ttu-id="cff77-106">Vyberte položku **poverenia systému Windows**.</span><span class="sxs-lookup"><span data-stu-id="cff77-106">Select **Windows Credentials**.</span></span>
1. <span data-ttu-id="cff77-107">Vyhľadajte ľubovoľnú položku, ktorá sa začína slovom **OneDrive**.</span><span class="sxs-lookup"><span data-stu-id="cff77-107">Find any entry that starts with the word **OneDrive**.</span></span>
1. <span data-ttu-id="cff77-108">Vyberte položku a potom stlačte kláves **odstrániť**.</span><span class="sxs-lookup"><span data-stu-id="cff77-108">Select the entry, then press **Remove**.</span></span>
1. <span data-ttu-id="cff77-109">Ukončite správcu poverení, kliknite pravým tlačidlom myši na modrý oblak v systray a vyberte položku **zatvorenie OneDrivu**.</span><span class="sxs-lookup"><span data-stu-id="cff77-109">Close Credential Manager, then right click on the blue cloud in your systray, and select **Close OneDrive**.</span></span>
1. <span data-ttu-id="cff77-110">Do vyhľadávacieho poľa na paneli úloh zadajte výraz **OneDrive** a výberom **aplikácie OneDrive** spustite OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cff77-110">Type **OneDrive** into the search box on the taskbar and select **OneDrive App** to launch OneDrive.</span></span>
1. <span data-ttu-id="cff77-111">Prihláste sa do služby OneDrive a potom sa pokúste súbor uložiť do služby OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cff77-111">Sign into OneDrive, then try to save the file to OneDrive.</span></span>
