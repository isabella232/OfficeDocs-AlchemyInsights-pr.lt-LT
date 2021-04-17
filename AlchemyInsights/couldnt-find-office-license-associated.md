---
title: "\"Microsoft 365\" programų taisymo nepavyko rasti su \"Office\" licencijomis susijusio pranešimo"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816496"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>"Microsoft 365" programų "Nepavyko rasti susietų "Office" licencijų" taisymo pranešimas

Jei gaunate šį pranešimą, bandykite atlikti šiuos veiksmus:

1. Patikrinkite užkardos, antivirusinės programinės įrangos ir tarpinio serverio parametrus, kad patvirtintumėte, jog jie neblokuoja interneto prieigos prie "Microsoft 365" programų. Žr. ["Microsoft 365" URL ir IP adresų diapazonai](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Pašalinkite [ir iš naujo priskirti susijusio vartotojo "Office"](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licenciją. 
3. Atidarykite "Office" programą [ir atsijungti](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) nuo esamų vartotojų paskyrų.
4. Eikite į "Windows" parametrai > **Paskyros**  >  **El. & paskyros** ir pašalinkite visas darbo paskyras, išskyrus paveiktą paskyrą.
5. Eikite į "Windows" parametrai >  >  **"Accounts Access" darbo arba mokymo** įstaigos ir atjunkite visas darbo paskyras, išskyrus paveiktą paskyrą.
6. Iš naujo nustatykite "Office" aktyvinimo būseną. [Sužinokite, kaip](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Prisijunkite naudodami](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) paveiktą vartotojo paskyrą.

Daugiau trikčių šalinimo sprendimų žr. [Nelicelicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).