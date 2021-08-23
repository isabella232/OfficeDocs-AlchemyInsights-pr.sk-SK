---
title: Vypnutie funkcií TLS1.0 a TLS 1.1 pre odosielanie klienta SMTP AUTH
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/18/2021
ms.locfileid: "58455124"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Vypnutie funkcií TLS1.0 a TLS 1.1 pre odosielanie klienta SMTP AUTH

Nedávno sme začali vypínať protokoly TLS1.0 a TLS 1.1 pre odosielanie klienta SMTP AUTH. 

Ak ste nakonfigurovali zariadenie, aplikáciu alebo server, ktoré odosiela e-maily do služieb Microsoft 365 pomocou metódy odosielania klienta SMTP AUTH, uistite sa, že vaše zariadenie, aplikácia alebo server podporujú protokol TLS 1.2 pre protokol SMTP. 