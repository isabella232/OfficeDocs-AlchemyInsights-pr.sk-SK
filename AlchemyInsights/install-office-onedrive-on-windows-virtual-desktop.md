---
title: Inštalácia balíka Office a OneDrivu vo virtuálnej pracovnej ploche Windowsu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596027"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Inštalácia balíka Office a OneDrivu vo virtuálnej pracovnej ploche Windowsu

1. [Pripravte a prispôsobte nadradený obrázok VHD.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image) Vytvorte virtuálny počítač (VM), ak ešte nebol vytvorený.

1. [Inštalácia balíka Office v režime aktivácie zdieľaného počítača.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) Aktivácia zdieľaného počítača umožňuje viacerým používateľom prístup k balíku Office.

1. [Nainštalujte OneDrive v režime pre počítač.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) Zvyčajne sa OneDrive inštaluje pre jedného používateľa, ale tu by sa mal nainštalovať do počítača.