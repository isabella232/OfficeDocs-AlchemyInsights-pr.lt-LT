---
title: Panaikintų vartotojų Microsoft 365 atkūrimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959034"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Panaikintų vartotojų Microsoft 365 atkūrimas

Galite atkurti panaikintus Microsoft 365 arba Microsoft Teams per 30 dienų nuo panaikinimo.

1. Eikite ["Microsoft 365" administravimo centras,](https://aka.ms/RestoreDeletedGroup) kad prisiregistruotų prie panaikintų grupių ir komandų sąrašo.

    **Pastaba:** Prisijunkite naudodami paskyrą, priskirtą nuomotojo administratoriui arba grupių administratoriaus vaidmeniui.

1. Pasirinkite panaikintus Microsoft 365 / Teams ir spustelėkite **atkurti grupę**.

    Jei grupės atkurti negalima dėl nesuderinamo SMTP adreso, naudokite šią komandą, kad rastumėte konfliktą keliantį objektą ir pašalintumėte SMTP adresą:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Pastaba:** Kai kuriais atvejais gali užtrukti iki 24 valandų, kol grupė ir visi jos duomenys bus atkurti.

    Daugiau informacijos arba sužinokite, kaip atkurti grupes naudojant "PowerShell", [žr. Panaikintų duomenų Microsoft 365 grupės atkūrimas.](https://go.microsoft.com/fwlink/?linkid=867802)