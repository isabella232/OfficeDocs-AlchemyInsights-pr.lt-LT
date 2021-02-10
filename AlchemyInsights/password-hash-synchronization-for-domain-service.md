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
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="11c31-102">Slaptažodžių maišos sinchronizavimo domeno tarnyba</span><span class="sxs-lookup"><span data-stu-id="11c31-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="11c31-103">**Jei jūsų "Azure AD DS" egzempliorius jums leidžia įgalinti slaptažodžių maišos sinchronizavimą**</span><span class="sxs-lookup"><span data-stu-id="11c31-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="11c31-104">Susidūrėte su scenarijumi, kuriame naudojate hibridinę aplinką su vartotojais, sinchronizuojant iš vietinio "Azure Active Directory" domenų tarnybos (AD DS) aplinkos.</span><span class="sxs-lookup"><span data-stu-id="11c31-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="11c31-105">Šis scenarijus aptinkamas nepaisant to, kad turite slaptažodžių maišos sinchronizavimą iš vietinio AD DS į "Azure AD" nuomotoją.</span><span class="sxs-lookup"><span data-stu-id="11c31-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="11c31-106">**Sukelti**</span><span class="sxs-lookup"><span data-stu-id="11c31-106">**Cause**</span></span>

<span data-ttu-id="11c31-107">Taip nutinka dėl to, kad "Azure AD Connect" nėra sinchronizuojama Senstelėjusi nauja technologija LAN Manager (NTLM) ir "Kerberos" slaptažodžių maišos, kurių reikia "Azure AD DS".</span><span class="sxs-lookup"><span data-stu-id="11c31-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="11c31-108">**Problemos**</span><span class="sxs-lookup"><span data-stu-id="11c31-108">**Workaround**</span></span> 

<span data-ttu-id="11c31-109">Jums reikės sukonfigūruoti "Azure AD Connect", kad sinchronizuotumėte šiuos slaptažodžius, reikalingus NTLM ir Kerberos autentifikavimui.</span><span class="sxs-lookup"><span data-stu-id="11c31-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="11c31-110">Sukonfigūravus "Azure AD Connect", vietinis abonemento kūrimo arba slaptažodžio keitimo įvykis taip pat sinchronizuojamas senstelėjusio slaptažodžio maišos su "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="11c31-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="11c31-111">[Čia](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) rasite daugiau informacijos apie tai ir patarimų, kaip įgalinti slaptažodžių sinchronizavimą "AZURE AD DS" hibridinėse aplinkose.</span><span class="sxs-lookup"><span data-stu-id="11c31-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>