---
title: Domenų tarnybos sinchronizavimas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885570"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="52439-102">Domenų tarnybos sinchronizavimas</span><span class="sxs-lookup"><span data-stu-id="52439-102">Domain service synchronization</span></span>

<span data-ttu-id="52439-103">"Azure Active Directory" domenų tarnybos ("Azure AD DS") valdomojo domeno objektai ir kredencialai gali būti sukurti vietiniame domene arba sinchronizuoti iš "Azure Active Directory" ("Azure AD") nuomotojo.</span><span class="sxs-lookup"><span data-stu-id="52439-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="52439-104">Kai pirmą kartą diegiate "Azure AD DS", automatiškai konfigūruojamas ir inicijuojamas automatinis vieno būdo sinchronizavimas, kad būtų galima replikuoti objektus iš "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="52439-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="52439-105">Šis vienkryptis sinchronizavimas toliau vykdomas fone, kad "Azure AD DS" valdomas domenas būtų atnaujintas su visais "Azure AD" pakeitimais.</span><span class="sxs-lookup"><span data-stu-id="52439-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="52439-106">Nėra sinchronizavimo su "Azure AD DS" atgal į "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="52439-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="52439-107">Daugiau informacijos apie "Azure Active Directory" domenų tarnybos sinchronizavimą rasite [domenų tarnybos sinchronizavimas](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="52439-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
