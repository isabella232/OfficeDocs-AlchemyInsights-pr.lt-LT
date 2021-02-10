---
title: Slaptažodžių maišos sinchronizavimo domeno tarnyba
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177486"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Slaptažodžių maišos sinchronizavimo domeno tarnyba

**Jei jūsų "Azure AD DS" egzempliorius jums leidžia įgalinti slaptažodžių maišos sinchronizavimą**

Susidūrėte su scenarijumi, kuriame naudojate hibridinę aplinką su vartotojais, sinchronizuojant iš vietinio "Azure Active Directory" domenų tarnybos (AD DS) aplinkos. Šis scenarijus aptinkamas nepaisant to, kad turite slaptažodžių maišos sinchronizavimą iš vietinio AD DS į "Azure AD" nuomotoją.

**Sukelti**

Taip nutinka dėl to, kad "Azure AD Connect" nėra sinchronizuojama Senstelėjusi nauja technologija LAN Manager (NTLM) ir "Kerberos" slaptažodžių maišos, kurių reikia "Azure AD DS".

**Problemos** 

Jums reikės sukonfigūruoti "Azure AD Connect", kad sinchronizuotumėte šiuos slaptažodžius, reikalingus NTLM ir Kerberos autentifikavimui.

Sukonfigūravus "Azure AD Connect", vietinis abonemento kūrimo arba slaptažodžio keitimo įvykis taip pat sinchronizuojamas senstelėjusio slaptažodžio maišos su "Azure AD". [Čia](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) rasite daugiau informacijos apie tai ir patarimų, kaip įgalinti slaptažodžių sinchronizavimą "AZURE AD DS" hibridinėse aplinkose.