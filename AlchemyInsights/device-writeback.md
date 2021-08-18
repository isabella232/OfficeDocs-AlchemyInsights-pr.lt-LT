---
title: Įrenginio writeback
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: c069d0b4588e53250d6cc1f3a66c744ea5c12ae4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320094"
---
# <a name="device-writeback"></a>Įrenginio writeback

Įrenginio "Writeback" naudojama šiais atvejais:

- Įjungti [Windows Hello verslui naudojant hibridinį sertifikato patikimumo diegimą](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Sąlyginės prieigos įgalinimas pagal įrenginius su ADFS (2012 R2 arba naujesnėmis) apsaugotomis programomis (pasitikėti šalių pasitikėjimais)

    **Pastaba:**"Azure AD" prenumerata Premium reikalinga įrenginio įrašymo atgal.

Tai suteikia papildomos saugos ir garantijos, kad prieiga prie taikomųjų programų suteikiama tik patikimiems įrenginiams. Daugiau informacijos apie sąlyginę prieigą žr. Rizikos valdymas naudojant [sąlyginę](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) prieigą ir vietinės sąlyginės prieigos nustatymas [naudojant ""Azure Active Directory" įrenginių registraciją](https://docs.microsoft.com/azure/active-directory/devices/overview).

Daugiau informacijos apie įrenginio rašymo atgalinio įrašymo įgalinimas įrenginiuose, žr. [Įrenginio rašymo atgalinio įrašymo įgalinimas](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).
