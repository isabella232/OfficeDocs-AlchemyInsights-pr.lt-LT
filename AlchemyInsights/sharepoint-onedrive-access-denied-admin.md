---
title: Prieigos uždraustų pranešimų trikčių diagnostika
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505387"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="63462-102">Prieigos uždraustų pranešimų trikčių šalinimas "Sharepoint" / "OneDrive" administravimo centre</span><span class="sxs-lookup"><span data-stu-id="63462-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="63462-103">Jei bandydami naršyti "Sharepoint" / "OneDrive" administravimo centre gaunate pranešimą apie prieigą, kuriai uždrausta, įsitikinkite, kad [vartotojui suteikėte licenciją](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="63462-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="63462-104">Jei vartotojas turi licenciją, taip pat turėtumėte įsitikinti, kad jam [priskirtas administratoriaus vaidmuo,](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) galintis pasiekti administravimo centrus.</span><span class="sxs-lookup"><span data-stu-id="63462-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="63462-105">Ši problema taip pat gali kilti, kai vartotojas yra panaikintas ir iš naujo sukurtas su tuo pačiu vartotojo vardą (UPN).</span><span class="sxs-lookup"><span data-stu-id="63462-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="63462-106">Nauja sąskaita sukuriama naudojant kitą PUID (paso unikalų ID) reikšmę.</span><span class="sxs-lookup"><span data-stu-id="63462-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="63462-107">Kai vartotojas bando pasiekti svetainių rinkinio arba jų "OneDrive", vartotojas yra neteisingas PUID.</span><span class="sxs-lookup"><span data-stu-id="63462-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="63462-108">Antrasis scenarijus apima katalogų sinchronizavimą su Active Directory organizacinio vieneto (OU).</span><span class="sxs-lookup"><span data-stu-id="63462-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="63462-109">Jei vartotojai jau prisijungė prie "SharePoint", o tada perkeliami į kitą OU ir sinchronizuojami su "SharePoint", jie gali susidurti su šia problema.</span><span class="sxs-lookup"><span data-stu-id="63462-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="63462-110">Norėdami išspręsti šią problemą, turite atkurti pradinį UPN su straipsnyje , [atkurti vartotojo "Microsoft 365".](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="63462-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="63462-111">Pastaba: jei "OneDrive" arba "SharePoint" administravimo centras nepasiekiamas keliems vartotojams, kurie anksčiau turėjo prieigą, gali būti laikina tarnybos problema.</span><span class="sxs-lookup"><span data-stu-id="63462-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="63462-112">[Patikrinkite tarnybos sveikatos ataskaitų sritį](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="63462-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


