---
title: Išbandyti IRM konfigūraciją, kad būtų galima naudoti naujas OME galimybes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812440"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Išbandyti IRM konfigūraciją, kad būtų galima naudoti naujas OME galimybes

Norėdami patikrinti, ar Microsoft 365 nuomotojas sukonfigūruotas naudoti naujas OME galimybes, prijungdami prie ["PowerShell" vykdykite šias "cmdlet" Exchange Online "PowerShell":](/powershell/exchange/exchange-online-powershell)


1. Patikrinkite savo nuomotojo IRM konfigūraciją paleisdami `Get-IRMConfiguration` . Įsitikinkite, kad šios reikšmės nustatytos kaip **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Naudodami domeną, siuntėjo adresą ir gavėją, paleiskite `Test-IRMConfiguration` . Jei testas nepraeina, ištirkite IRM konfigūraciją.

Daugiau informacijos, kaip patikrinti IRM konfigūraciją, žr. Naujos OME konfigūracijos [tikrinimas "Exchange Online PowerShell".](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)