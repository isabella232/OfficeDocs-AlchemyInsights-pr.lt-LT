---
title: Saugos patarimo trikčių diagnostika tikrinant sukčiavimą
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504991"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Saugos patarimo trikčių diagnostika tikrinant sukčiavimą

Jei gaunate saugos patarimą, kuriame sakoma: "Siuntėjas nepavyko aptikti mūsų sukčiavimo ir gali būti ne tai, kas jie atrodo", siuntėjui nepavyko perduoti DKIM arba SPF autentifikavimo patikrinimų. Geriausias būdas išspręsti šią problemą yra siuntėjas turi teisę patys. Jei siuntėjas siunčia jūsų vardu, turite jį įgalioti įtraukdami siuntėjo IP adresą į savo SPF įrašą.
  
Daugiau informacijos rasite [Raudonojo (įtartino) saugos patarimo trikčių diagnostika.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)
  
Štai keletas kitų nuorodų, kurios gali padėti:
  
- [Kaip "Microsoft" naudoja siuntėjo strategijos sistemą (SPF) išvengti apsiausto](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF nustatymas, kad būtų išvengta apsiausto](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
