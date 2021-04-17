---
title: Apgaulės aptikimo tikrinimo saugos patarimo trikčių šalinimas
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834739"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Apgaulės aptikimo tikrinimo saugos patarimo trikčių šalinimas

Jei gaunate saugos patarimą, kuriame rašoma: "Siuntėjui nepavyko aptikti sukčiavimo ir jis gali būti ne toks, kaip jis atrodo", siuntėjui nepavyko atlikti DKIM arba SPF autentifikavimo patikrų. Geriausias būdas išspręsti šią problemą yra leisti siuntėjui. Jei siuntėjas siunčia jūsų vardu, turite jį autorizuoti įtraukdami siuntėjo IP adresą į SAVO SPF įrašą.
  
Daugiau [informacijos žr. Raudono (įtartinos) saugos patarimo trikčių](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) šalinimas, kad būtų galima aptikti apgaulės atvejus.
  
Štai keletas kitų saitų, kurie gali padėti:
  
- [Kaip "Microsoft" naudoja siuntėjų strategijos sistemą (SPF), kad išvengtų sąsojimo](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF, kad būtų užkirstas kelias spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
