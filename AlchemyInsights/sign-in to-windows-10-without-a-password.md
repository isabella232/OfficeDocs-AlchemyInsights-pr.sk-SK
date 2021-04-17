---
title: Prihlásenie do Windowsu 10 bez použitia hesla
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830561"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="f1edf-102">Prihlásenie do Windowsu 10 bez použitia hesla</span><span class="sxs-lookup"><span data-stu-id="f1edf-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="f1edf-103">Ak sa chcete vyhnúť nutnosti písať heslo pri spustení Windowsu, odporúčame použiť niektorú z možností prihlásenia prostredníctvom funkcie Windows Hello, ako je napríklad PIN kód, rozpoznávanie tváre alebo odtlačok prsta, ak sú k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="f1edf-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="f1edf-104">Ak naozaj chcete vypnúť zabezpečené prihlásenie, pozrite si nižšie uvedené pokyny Automaticky sa prihlásiť do Windowsu 10.</span><span class="sxs-lookup"><span data-stu-id="f1edf-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="f1edf-105">**Zabezpečenie alternatívy funkcie Windows Hello k hesle konta**</span><span class="sxs-lookup"><span data-stu-id="f1edf-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="f1edf-106">Prejdite na **položky > Kontá > Možnosti prihlásenia** (alebo kliknite [sem](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="f1edf-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="f1edf-107">Zobrazí sa zoznam dostupných možností prihlásenia.</span><span class="sxs-lookup"><span data-stu-id="f1edf-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="f1edf-108">Príklad:</span><span class="sxs-lookup"><span data-stu-id="f1edf-108">For example:</span></span>

![Možnosti prihlásenia.](media/sign-in-options.png)

<span data-ttu-id="f1edf-110">Kliknutím alebo ťuknutím na niektorú z možností ju nakonfigurujte.</span><span class="sxs-lookup"><span data-stu-id="f1edf-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="f1edf-111">Pri ďalšom spustení alebo odomknutí Windowsu budete môcť namiesto hesla použiť novú možnosť.</span><span class="sxs-lookup"><span data-stu-id="f1edf-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="f1edf-112">**Automatické prihlásenie do Windowsu 10**</span><span class="sxs-lookup"><span data-stu-id="f1edf-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="f1edf-113">**Poznámka:** Automatické prihlásenie je praktické, ale predstavuje riziko zabezpečenia, najmä ak k počítaču pristupuje viacero ľudí.</span><span class="sxs-lookup"><span data-stu-id="f1edf-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="f1edf-114">Kliknite alebo ťuknite **na tlačidlo** Štart na paneli úloh.</span><span class="sxs-lookup"><span data-stu-id="f1edf-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="f1edf-115">Zadajte **text netplwiz** a stlačením klávesu Enter otvorte okno Používateľské kontá.</span><span class="sxs-lookup"><span data-stu-id="f1edf-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="f1edf-116">V **časti Používateľské kontá** kliknite na konto, do ktorého sa chcete automaticky prihlasovať pri spustení Windowsu.</span><span class="sxs-lookup"><span data-stu-id="f1edf-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="f1edf-117">Zrušte začiarknutie políčka Ak chcete používať tento počítač, používatelia musia zadať meno používateľa a heslo.</span><span class="sxs-lookup"><span data-stu-id="f1edf-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Používatelia musia zadať možnosť používateľského mena a hesla.](media/users-must-enter-username.png)

5. <span data-ttu-id="f1edf-119">Kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="f1edf-119">Click **OK**.</span></span> <span data-ttu-id="f1edf-120">Zobrazí sa výzva na zadanie a potvrdenie hesla pre vybraté konto.</span><span class="sxs-lookup"><span data-stu-id="f1edf-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="f1edf-121">**Dokončite kliknutím** na tlačidlo OK.</span><span class="sxs-lookup"><span data-stu-id="f1edf-121">Click **OK** to finish.</span></span> <span data-ttu-id="f1edf-122">Pri ďalšom spustení Windowsu 10 sa automaticky prihlási do vybratého konta.</span><span class="sxs-lookup"><span data-stu-id="f1edf-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
