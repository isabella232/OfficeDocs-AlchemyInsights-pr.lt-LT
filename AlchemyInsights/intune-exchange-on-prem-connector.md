---
title: "\"Intune Exchange vietinė jungtis"
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
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013972"
---
# <a name="intune-exchange-on-premise-connector"></a>"Intune Exchange vietinė jungtis

Išsamesnės informacijos, kaip nustatyti jungtį tarp "Intune" ir "Exchange, kurios ištekliai nuomojami vietoje, ieškokite šioje dokumentacijoje:

[Vietinės "Intune" jungties Exchange ""Microsoft Intune" Azure"](https://docs.microsoft.com/intune/exchange-connector-install)

**DUK:**

K: matau klaidą, pvz., "Exchange jungties versija nepalaikoma" bandant nustatyti Exchange jungtį. Kokia gali būti priežastis?

A: jūsų naudojama paskyra tinkamai licencijuota – ji turi turėti aktyvią "Intune" licenciją

K: Ar galima turėti kelias Exchange jungtis?

A: Galite nustatyti tik vieną Exchange jungtį vienam "Intune" nuomotojui Exchange organizacijoje. Jungtį galima įdiegti tik viename kelių serverių mainų organizacijos serveryje.

Taip pat negalite sukonfigūruoti jungčių, Exchange vietiniame ir Exchange Online tame pačiame nuomotoje.

K: ar jungtis gali naudoti CAS masyvą kaip ryšį su Exchange?

A: CAS masyvo nurodymas jungties sąrankoje nėra palaikoma konfigūracija. Turi būti nurodytas tik vienas serveris ir jis turėtų būti užkoduotas jungties konfigūracijos faile, kurį galima rasti

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Raskite šį įrašą ```<ExchangeWebServiceURL />``` ir pakeiskite URL "Exchange" serveriu.

**Pavyzdys:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Daugiau trikčių diagnostikos žr. šioje dokumentacijoje: [Vietinės "Intune"](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune) Exchange trikčių šalinimas

**Daugiažodės jungties daugiažodinio Exchange įgalinimas**

1. Atidarykite Exchange jungties sekimo konfigūracijos failą, kad jį būtų galima redaguoti.  
Failas yra : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Pavyzdys:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Raskite TraceSourceLine naudodami šį raktą: OnPremisesExchangeConnectorService  
  
3. Mazgo SourceLevel reikšmės keitimas iš Informacijos veiklaSątrauka (numatytoji reikšmė) į Išsami veiklaSątrauka  

**Pavyzdys:**
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
4. Iš naujo paleiskite "Microsoft Intune" Exchange tarnybą  
5. Visiškas sinchronizavimas "Intune" portale, kol jis baigsis, tada pakeiskite XML atgal į "Information ActivityTracing" ir iš naujo paleiskite "Microsoft Intune" Exchange tarnybą.  
6. Žurnalų vieta yra: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`