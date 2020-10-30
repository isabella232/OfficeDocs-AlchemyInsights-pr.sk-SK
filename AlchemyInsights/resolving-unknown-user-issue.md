---
title: Riešenie problému s neznámym používateľom v chate v aplikácii teams
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003807"
- "6809"
ms.openlocfilehash: 523c11cb9d5c4696703c67c2a6b3184f5d12f8e7
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807773"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a><span data-ttu-id="d708d-102">Riešenie problému s výrazom Neznámy používateľ v aplikácii teams chat</span><span class="sxs-lookup"><span data-stu-id="d708d-102">Resolving issue with "Unknown User" in Teams Chat</span></span>

<span data-ttu-id="d708d-103">V niektorých časoch sa odstránený používateľ zobrazí ako Neznámy používateľ.</span><span class="sxs-lookup"><span data-stu-id="d708d-103">At times, a removed user will appear as "Unknown User".</span></span> <span data-ttu-id="d708d-104">Toto je [známy problém](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span><span class="sxs-lookup"><span data-stu-id="d708d-104">This is a [known issue](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span></span>

<span data-ttu-id="d708d-105">Ak sa stále zobrazuje používateľom v chatoch v aplikácii teams ako Neznámy používateľ, vyskúšajte a vymažte vyrovnávaciu pamäť:</span><span class="sxs-lookup"><span data-stu-id="d708d-105">If you are persistently seeing users showing as "Unknown User" in Teams chats, try and clear the cache:</span></span>

1.  <span data-ttu-id="d708d-106">Kliknite pravým tlačidlom myši na ikonu teams na paneli úloh.</span><span class="sxs-lookup"><span data-stu-id="d708d-106">Right-click the Teams icon in the taskbar.</span></span> <span data-ttu-id="d708d-107">Kliknite na položku  **skončiť** .</span><span class="sxs-lookup"><span data-stu-id="d708d-107">Click  **Quit** .</span></span>
2.  <span data-ttu-id="d708d-108">Prejdite do priečinka%appdata%\Microsoft\teams\ v počítači a odstráňte všetky súbory v danom adresári.</span><span class="sxs-lookup"><span data-stu-id="d708d-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>

<span data-ttu-id="d708d-109">Anonymným používateľom môžete zabrániť v pripojení k schôdzi tak, že ich počkáte v lobby.</span><span class="sxs-lookup"><span data-stu-id="d708d-109">You can prevent anonymous users from joining meetings by ensuring that they wait in the lobby.</span></span> <span data-ttu-id="d708d-110">Ďalšie informácie nájdete v téme [Zmena nastavení účastníkov schôdze cez Team](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span><span class="sxs-lookup"><span data-stu-id="d708d-110">For more information, see [Change participant settings for a Teams meeting](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span></span>
