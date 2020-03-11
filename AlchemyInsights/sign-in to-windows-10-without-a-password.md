---
title: Prihlásenie do systému Windows 10 bez použitia hesla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588295"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="aefe1-102">Prihlásenie do systému Windows 10 bez použitia hesla</span><span class="sxs-lookup"><span data-stu-id="aefe1-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="aefe1-103">Ak sa chcete vyhnúť nutnosti zadávať heslo pri spustení systému Windows, odporúčame vám použiť jeden z možností na prihlasovanie v programe Windows Hello, ako je napríklad kód PIN, rozpoznávanie tvárí alebo odtlačok prsta, ak je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="aefe1-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="aefe1-104">Ak naozaj chcete zakázať bezpečné prihlasovanie, pozrite si nižšie uvedené pokyny "automaticky sa prihlásiť do Windowsu 10".</span><span class="sxs-lookup"><span data-stu-id="aefe1-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="aefe1-105">**Bezpečné Windows Hello alternatívy k heslu účtu**</span><span class="sxs-lookup"><span data-stu-id="aefe1-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="aefe1-106">Prejdite do **časti nastavenia > kontá > možnosti prihlásenia** (alebo kliknite [sem](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="aefe1-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="aefe1-107">Dostupné možnosti prihlásenia budú uvedené.</span><span class="sxs-lookup"><span data-stu-id="aefe1-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="aefe1-108">Príklad:</span><span class="sxs-lookup"><span data-stu-id="aefe1-108">For example:</span></span>

![Možnosti prihlásenia.](media/sign-in-options.png)

<span data-ttu-id="aefe1-110">Kliknite alebo ťuknite na niektorú z možností, ktoré chcete nakonfigurovať.</span><span class="sxs-lookup"><span data-stu-id="aefe1-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="aefe1-111">Pri ďalšom spustení alebo odomknutí systému Windows budete môcť namiesto hesla použiť novú možnosť.</span><span class="sxs-lookup"><span data-stu-id="aefe1-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="aefe1-112">**Automatické prihlásenie do Windowsu 10**</span><span class="sxs-lookup"><span data-stu-id="aefe1-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="aefe1-113">**Poznámka**: automatické prihlasovanie je výhodné, ale zavádza bezpečnostné riziko, najmä ak je váš počítač prístupný viacerým ľuďom.</span><span class="sxs-lookup"><span data-stu-id="aefe1-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="aefe1-114">Kliknite alebo ťuknite na tlačidlo **Štart** na paneli úloh.</span><span class="sxs-lookup"><span data-stu-id="aefe1-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="aefe1-115">Typ **netplwiz** a stlačte klávesu Enter otvorte okno Používateľské kontá.</span><span class="sxs-lookup"><span data-stu-id="aefe1-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="aefe1-116">V **používateľských kontách**kliknite na konto, do ktorého sa chcete automaticky prihlásiť pri spustení systému Windows.</span><span class="sxs-lookup"><span data-stu-id="aefe1-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="aefe1-117">Zrušte začiarknutie políčka "používatelia musia zadať meno používateľa a heslo na používanie tohto počítača" začiarkavacie políčko.</span><span class="sxs-lookup"><span data-stu-id="aefe1-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Používatelia musia zadať užívateľské meno a heslo možnosť.](media/users-must-enter-username.png)

5. <span data-ttu-id="aefe1-119">Kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="aefe1-119">Click **OK**.</span></span> <span data-ttu-id="aefe1-120">Zobrazí sa výzva na zadanie a potvrdenie hesla pre konto, ktoré ste vybrali.</span><span class="sxs-lookup"><span data-stu-id="aefe1-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="aefe1-121">Kliknite na **tlačidlo OK** dokončiť.</span><span class="sxs-lookup"><span data-stu-id="aefe1-121">Click **OK** to finish.</span></span> <span data-ttu-id="aefe1-122">Pri ďalšom spustení systému Windows 10 sa automaticky prihlásite do vybratého konta.</span><span class="sxs-lookup"><span data-stu-id="aefe1-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
