---
title: Trikčių šalinimo problema – vartotojas nerastas kataloge
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098178"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Trikčių šalinimo problema – vartotojas nerastas kataloge

Jei vartotojai gauna klaidos pranešimą "nepavyko rasti vartotojo" kataloge, bandykite dar kartą, kai problemos tipas yra Vartotojas, kuris nėra kataloge.

Norėdami išspręsti šią problemą, galite atlikti šiuos veiksmus.

- Įsitikinkite, kad paskyra, kuri priėmė kvietimą el. paštu, yra ta pati paskyra, kuri naudojama prisijungti vėliau. Įsitikinkite, kad vartotojas naudoja tą pačią paskyrą kvietimui priimti ir prisijungti prie svetainės. 

Daugiau informacijos žr. [Kaip valdyti "Microsoft" paskyros </a> pseudonimus, kad valdytumėte Microsoft 365 prisijungimą](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Eikite į kiekvieną svetainę (-es), kurioje (-ias) vartotojas gauna klaidą. 

Įtraukite "/_layouts/15/people.aspx/membershipgroupid=0" (dvigubose kabutėse) į svetainės URL pabaigą. 

Pavyzdys: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Pasirinkite vartotoją iš sąrašo.

- Juostelėje **spustelėkite Šalinti** vartotojo teises. 
-  Įtraukite atgal į vartotoją ir iš naujo iš naujo siųskite kvietimą vartotojui.

