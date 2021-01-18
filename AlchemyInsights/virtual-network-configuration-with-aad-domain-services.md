---
title: Virtuali konfigūracija su "AAD" domenų tarnybomis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885643"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuali konfigūracija su "AAD" domenų tarnybomis

Virtualioji konfigūracija su "AAD" domenų tarnybomis apima šiuos veiksmus: 

1. Domeno sveikatos tikrinimas "Azure" portale https://aka.ms/aadds-health
2. "NSG" tikrinimo taisyklės, kurios blokuoja prievadus, reikalingus sinchronizuoti "Azure AD" domenų tarnybose portale https://aka.ms/aadds-networking
3. Užtikrinti, kad jūsų virtualus tinklas būtų įdiegtas tame pačiame "Azure" regione kaip jūsų "Azure AD" domenų tarnybos valdomas domenas.
4. Užtikrinti, kad neturite esamo domeno su tuo pačiu domeno pavadinimu, kurį galima naudoti virtualiame tinkle.

Daugiau informacijos apie dizaino atlygį "Azure" virtualiame tinkle, siekiant palaikyti "AAD" domenų tarnybas, ieškokite [virtualiojo tinklo nagrinėjimo](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

