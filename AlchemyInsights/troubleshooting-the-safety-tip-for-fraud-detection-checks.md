---
title: Saugos patarimo dėl sukčiavimo aptikimo patikrų trikčių diagnostika
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658418"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Saugos patarimo dėl sukčiavimo aptikimo patikrų trikčių diagnostika

Jei gaunate saugos patarimą, kuriame rašoma: "siuntėjas nesugebėjo atlikti apgaulės aptikimo patikrų ir gali būti ne tas, kas jie atrodo", tada siuntėjui nepavyko perduoti DKIM arba SPF autentifikavimo. Geriausias būdas išspręsti šią problemą yra tas, kad siuntėjas turi sau leisti. Jei siuntėjas siunčia jūsų vardu, turite juos įgalioti, įtraukdami siuntėjo IP adresą į savo SPF įrašą.
  
Sužinokite daugiau informacijos apie " [Red (įtartiną) saugos patarimo dėl sukčiavimo aptikimo trikčių diagnostiką](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Štai keletas kitų saitų, kurie gali padėti:
  
- [Kaip "Microsoft" naudoja siuntėjo strategijos programą (SPF), kad užkirstų kelią "spoofing"](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- ["SPF" nustatymas, padėsianti apsisaugoti nuo apsimetimo kitu](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
