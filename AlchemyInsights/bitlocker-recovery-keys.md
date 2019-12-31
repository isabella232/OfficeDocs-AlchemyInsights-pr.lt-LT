---
title: "\"BitLocker\" atkūrimo raktai"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908822"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="1bde1-102">Prieiga prie "BitLocker" atkūrimo raktų</span><span class="sxs-lookup"><span data-stu-id="1bde1-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="1bde1-103">Konfigūruojant BitLocker parametrus Intune Endpoint Protection strategijos, galima nustatyti, ar "BitLocker" atkūrimo informacija turi būti saugoma Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1bde1-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="1bde1-104">Jei šis parametras sukonfigūruotas, saugomi atkūrimo duomenys turi būti matomi Intune administratorius kaip įrenginio įrašo duomenų Intune įrenginių ašmenys dviem būdais:</span><span class="sxs-lookup"><span data-stu-id="1bde1-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="1bde1-105">Įrenginiai – "Azure AD" įrenginiai – > "įrenginys" arba įrenginiai – > visi įrenginiai – > "įrenginys" – > atkūrimo raktai</span><span class="sxs-lookup"><span data-stu-id="1bde1-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="1bde1-106">Arba, jei yra administratoriaus prieigos prie paties įrenginio, atkūrimo rakto (slaptažodis) galima matyti vykdydami šią komandą iš didesnių teisių komandų eilutėje:</span><span class="sxs-lookup"><span data-stu-id="1bde1-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="1bde1-107">Jei įrenginys buvo užšifruotas prieš registracija į Intune, atkūrimo raktas gali būti susietas su "Microsoft account" (MSA), naudojama prisijungti prie įrenginio OOBE metu.</span><span class="sxs-lookup"><span data-stu-id="1bde1-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="1bde1-108">Tokiu atveju norint pasiekti https://onedrive.live.com/recoverykey ir prisijungti prie MSA turėtų būti rodomi įrenginiai, kuriems atkūrimo raktai buvo saugomi.</span><span class="sxs-lookup"><span data-stu-id="1bde1-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="1bde1-109">Jei įrenginys buvo užšifruotas dėl konfigūracijos naudojant domeno grupės strategiją, atkūrimo informacija gali būti saugoma vietiniame Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1bde1-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

