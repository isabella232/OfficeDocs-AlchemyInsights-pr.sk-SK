---
title: Ontune Exchange on-premise Connector
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013979"
---
# <a name="intune-exchange-on-premise-connector"></a>Ontune Exchange on-premise Connector

Podrobnosti o nastavení konektora medzi služby Intune a Exchange, ktorý je hosťovaný lokálne, nájdete v nasledujúcej dokumentácii:

[Nastavenie lokálneho konektora Intune Exchange v Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**Najčastejšie otázky:**

Otázka: Pri pokuse o nastavenie spojnice sa zobrazí chyba, ako je napríklad Exchange Exchange konektor, nie je podporovaný. Čo to môže byť príčina?

A: Konto, ktoré používate, má príslušnú licenciu – musí mať aktívnu licenciu služby Intune

Otázka: Je možné mať viacero spojníc Exchange údajov?

A: Pre jednu organizáciu môžete nastaviť Exchange konektora pre jedného nájomníka služby Intun Exchange e. Konektor môže byť nainštalovaný len na jednom serveri v organizácii s viacerými servermi na výmenu.

Konektory nie je možné nakonfigurovať pre Exchange pre server a konektory Exchange Online nakonfigurované v tom istom nájomníkovi.

Otázka: Môže spojnica použiť pole CAS ako svoje pripojenie k Exchange?

A: Zadanie poľa CAS nie je podporovaná konfigurácia v nastavení konektora. Mal by byť zadaný len jeden server a mal by byť kódovaný v konfiguračnom súbore konektora, ktorý nájdete v časti

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Vyhľadajte nasledujúcu položku ```<ExchangeWebServiceURL />``` a nahraďte URL adresu Exchange Serverom.

**Príklad:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Ďalšie riešenie problémov nájdete v nasledujúcej dokumentácii: [Riešenie problémov s lokálnym konektorom intune Exchange.](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Povolenie zapisovania slovesného zapisovania do Exchange spojnice**

1. Na úpravy otvorte súbor Exchange Connector tracing.  
Súbor sa nachádza na adrese : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Príklad:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Vyhľadajte položku TraceSourceLine pomocou tohto kľúča: OnPremisesExchangeConnectorService  
  
3. Zmena hodnoty uzla SourceLevel z Information ActivityTracing (predvolené) na Verbose ActivityTracing  

**Príklad:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Reštartujte službu Microsoft Intune Exchange zariadenia  
5. Úplná synchronizácia na portáli Intune, kým sa nedokončí, a potom zmeňte XML súbor späť na information activitytracing a reštartujte Microsoft Intune Exchange služby.  
6. Umiestnenie denníkov je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`