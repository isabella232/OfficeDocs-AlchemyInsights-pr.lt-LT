---
title: Trikčių diagnostika – vartotojas nerastas kataloge
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702746"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Trikčių diagnostika – vartotojas nerastas kataloge

Jei vartotojai gauna klaidos pranešimą "vartotojas negali būti rastas" kataloge, bandykite dar kartą, kai problemos tipas yra vartotojo nėra kataloge.

Norėdami išspręsti šią problemą, galima atlikti šiuos veiksmus.

- Įsitikinkite, kad paskyrą, kuri priėmė kvietimą el. paštu, yra ta pati paskyra, kuri naudojama prisijungti vėliau. Įsitikinkite, kad vartotojas naudoja tą patį abonementą, kad priimtų kvietimą ir prisijungtumėte prie svetainės. 

Daugiau informacijos rasite [Kaip tvarkyti "Microsoft" paskyros</a> pseudonimus, kad galėtumėte valdyti "Microsoft 365" prisijungimą](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Pereikite prie kiekvienos (-ių) svetainės (-ių), kurioje (-iose) vartotojas gauna klaidą. 

Pridėti "/_layouts/15/people.aspx/membershipgroupid=0" (per dvigubas kabutes) svetainės URL pabaigoje. 

Pavyzdys: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Pasirinkite vartotoją iš sąrašo.

- Juostelėje spustelėkite **Šalinti vartotojo teises.** 
-  Pridėkite atgal vartotoją ir iš naujo nusiųskite kvietimą vartotojui.

