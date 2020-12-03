---
title: Naikinti nuomotoją
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564616"
---
# <a name="delete-tenant"></a><span data-ttu-id="c44fc-102">Naikinti nuomotoją</span><span class="sxs-lookup"><span data-stu-id="c44fc-102">Delete tenant</span></span>

<span data-ttu-id="c44fc-103">Norėdami panaikinti "Azure AD", įsitikinkite, kad:</span><span class="sxs-lookup"><span data-stu-id="c44fc-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="c44fc-104">Esate visuotinis administratorius kataloge.</span><span class="sxs-lookup"><span data-stu-id="c44fc-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="c44fc-105">Nesate prisijungę naudodami paskyrą, kurioje yra numatytasis katalogas, pvz., "contoso.onmicrosoft.com", prisijungęs prie paskyros, pvz., "admin@contoso.onmicrosoft.com".</span><span class="sxs-lookup"><span data-stu-id="c44fc-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="c44fc-106">Pašalinkite visas aktyvias taikomąsias programas kataloge prieš ištrindami.</span><span class="sxs-lookup"><span data-stu-id="c44fc-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="c44fc-107">Norėdami pašalinti aktyvias taikomąsias programas, pereikite prie taikomųjų programų registracijų ir pašalinkite esamas taikomąsias programas.</span><span class="sxs-lookup"><span data-stu-id="c44fc-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="c44fc-108">Nėra jokių aktyvių "Microsoft Online Services" prenumeratų, pvz., "Microsoft Azure", "Office 365" arba "Azure AD Premium".</span><span class="sxs-lookup"><span data-stu-id="c44fc-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="c44fc-109">Perkelkite savo prenumeratas arba Paspartinkite aktyvių prenumeratų panaikinimą naudodami "Azure" palaikymą ir atsiskaitymą.</span><span class="sxs-lookup"><span data-stu-id="c44fc-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="c44fc-110">Sužinokite daugiau, kaip atšaukti "Office 365" ir "Azure" prenumeratas.</span><span class="sxs-lookup"><span data-stu-id="c44fc-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="c44fc-111">Nurodymų, kaip susieti arba įtraukti esamą prenumeratą į nuomotoją, ieškokite "Azure [AD" nuomotojui susiekite arba įtraukite "Azure" prenumeratą](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="c44fc-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="c44fc-112">Nėra aktyvios licencijos.</span><span class="sxs-lookup"><span data-stu-id="c44fc-112">There are no Active license.</span></span> <span data-ttu-id="c44fc-113">Norėdami pašalinti licencijas, Sužinokite, [kaip pašalinti prenumeratą, kad pašalintumėte licenciją](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="c44fc-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="c44fc-114">Kataloge nėra kitų aktyvių vartotojų, išskyrus save kaip visuotinį administratorių, bandant panaikinti "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="c44fc-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="c44fc-115">Pašalinti visus kitus aktyvius vartotojus ir bet kurią priklausomybes, esančias pasirinktinio domeno varde nuomotojuje, taip pat reikės pašalinti, pvz., "admin@contoso.com" sukurtus vartotojus.</span><span class="sxs-lookup"><span data-stu-id="c44fc-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="c44fc-116">Daugiau informacijos apie tai, kaip:</span><span class="sxs-lookup"><span data-stu-id="c44fc-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="c44fc-117">Naikinti "Azure Active Directory" arba "prenumerata", rasite " [Azure Active Directory" naikinimas](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="c44fc-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="c44fc-118">Pašalinti taikomąsias programas kataloge rasite [taikomųjų programų šalinimas](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="c44fc-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
