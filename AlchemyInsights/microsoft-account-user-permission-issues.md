---
title: Trikčių šalinimo problema – vartotojas kataloge nerastas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725415"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Trikčių šalinimo problema – vartotojas kataloge nerastas

Jei vartotojai gauna klaidos pranešimą "vartotojas negali būti rastas" kataloge, bandykite dar kartą, kai problemos tipas yra vartotojo kataloge nėra.

Toliau nurodytus veiksmus galima atlikti, kad išspręstumėte problemą.

- Įsitikinkite, kad abonementas, kuris priėmė kvietimą į laišką, yra ta pati paskyra, kuri yra naudojama prisijungiant. Įsitikinkite, kad vartotojas naudoja tą pačią paskyrą, kad priimtų kvietimą ir prisijungtų prie svetainės. 

Daugiau informacijos ieškokite [kaip valdyti "Microsoft" paskyros pseudonimus, </a> kad galėtumėte valdyti "microsoft" 365 prisijungimą](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Eikite į kiekvieną svetainę (-as), kurioje vartotojas gauna klaidą. 

Įtraukite "/_layouts/15/People.aspx/membershipgroupid = 0" (per dvigubų kabučių) į svetainės URL pabaigą. 

Pavyzdys: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Sąraše pasirinkite vartotoją.

- Juostelėje spustelėkite **pašalinti vartotojų teises** . 
-  Įtraukti vartotoją ir iš naujo persiųsti kvietimą vartotojui.

