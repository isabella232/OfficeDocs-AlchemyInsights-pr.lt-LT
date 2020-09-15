---
title: "\"BitLocker\" atkūrimo raktai"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685894"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="15da4-102">Prieiga prie "BitLocker" atkūrimo raktų</span><span class="sxs-lookup"><span data-stu-id="15da4-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="15da4-103">Konfigūruojant "BitLocker" parametrų Intune Endpoint Protection strategiją, galima nustatyti, ar "BitLocker" atkūrimo informacija turėtų būti saugoma "Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="15da4-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="15da4-104">Jei šis parametras sukonfigūruotas, saugomi atkūrimo duomenys turėtų būti matomi Intune admin kaip įrenginio įrašo duomenis "Intune" įrenginių ašmenimis dviem būdais:</span><span class="sxs-lookup"><span data-stu-id="15da4-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="15da4-105">Įrenginiai – "Azure AD" įrenginiai – > "įrenginys" arba įrenginiai – > visi įrenginiai – > "įrenginys" – > atkūrimo raktai</span><span class="sxs-lookup"><span data-stu-id="15da4-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="15da4-106">Arba, jei yra administracinė prieiga prie paties įrenginio, atkūrimo raktą (slaptažodį) galima matyti paleisdami šią komandą iš didesnių teisių komandų eilutės:</span><span class="sxs-lookup"><span data-stu-id="15da4-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="15da4-107">Jei įrenginys buvo užšifruotas prieš registraciją "Intune", atkūrimo kodas gali būti susietas su "Microsoft" abonementu (MSA), naudojamu prisijungti prie įrenginio OOBE proceso metu.</span><span class="sxs-lookup"><span data-stu-id="15da4-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="15da4-108">Jei tai buvo atvejis, prisijungimas prie  https://onedrive.live.com/recoverykey MSA ir prisijungimas prie jos turėtų Rodyti įrenginius, kurių atkūrimo raktai buvo saugomi.</span><span class="sxs-lookup"><span data-stu-id="15da4-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="15da4-109">Jei įrenginys buvo užšifruotas kaip konfigūravimo rezultatas pagal domeno grupės strategiją, atkūrimo informacija gali būti saugoma vietiniame "Active Directory".</span><span class="sxs-lookup"><span data-stu-id="15da4-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

