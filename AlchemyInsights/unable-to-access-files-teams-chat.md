---
title: Nie je možné získať prístup k súborom zdieľaným v chate v Teams
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/02/2021
ms.locfileid: "51596012"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a><span data-ttu-id="73490-102">Nie je možné získať prístup k súborom zdieľaným v chate v Teams</span><span class="sxs-lookup"><span data-stu-id="73490-102">Unable to access files shared in Teams chat</span></span>

<span data-ttu-id="73490-103">V aplikácii Microsoft Teams sa súbor zdieľaný používateľom v okne chatu automaticky uloží na lokalite OneDrive zdieľaného používateľa.</span><span class="sxs-lookup"><span data-stu-id="73490-103">In Microsoft Teams, a file shared by a user in a chat window is stored automatically on the sharing user's OneDrive site.</span></span>

<span data-ttu-id="73490-104">Keď sa iný používateľ pokúsi otvoriť súbor v aplikácii Teams a zobrazí sa chybové hlásenie "Nemáte prístup k tomuto súboru", tento problém sa vyskytuje, pretože na vašej lokalite OneDrive je aktivovaná funkcia režimu uzamknutia s povolením obmedzeného prístupu používateľa.</span><span class="sxs-lookup"><span data-stu-id="73490-104">When another user tries to open the file in Teams and receives the error message "You don't have access to this file," the issue occurs because the Limited-access user permission lockdown mode feature is activated on your OneDrive site.</span></span>

1. <span data-ttu-id="73490-105">Pokyny na vypnutie funkcie na lokalite OneDrive nájdete v téme Chyba [pri otváraní súboru v aplikácii Teams.](https://go.microsoft.com/fwlink/?linkid=2155733)</span><span class="sxs-lookup"><span data-stu-id="73490-105">For instructions to disable the feature on the OneDrive site, see [Error when opening a file in Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span></span>

1. <span data-ttu-id="73490-106">Skontrolujte, či má k lokalite OneDrive prístup iný používateľ, a poskytujte prístup podľa pokynov v časti Zdieľanie súborov a priečinkov [vo OneDrive.](https://go.microsoft.com/fwlink/?linkid=2156017)</span><span class="sxs-lookup"><span data-stu-id="73490-106">Check whether another user has access to the OneDrive site, and provide access by following the instructions in [Share OneDrive files and folders](https://go.microsoft.com/fwlink/?linkid=2156017).</span></span>