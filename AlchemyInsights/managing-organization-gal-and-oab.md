---
title: Organizacijos visuotinio adresų sąrašo ir autonominės adresų knygelės valdymas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022523"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="4457a-102">Organizacijos visuotinio adresų sąrašo (GAL) ir autonominės adresų knygelės valdymas (OAB)</span><span class="sxs-lookup"><span data-stu-id="4457a-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="4457a-103">Visuotinis adresų sąrašas (GAL) yra objektų, kuriuose įgalintas el. paštas, sąrašas (bet kokio tipo gavėjas, kuris gali gauti el. laišką) organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="4457a-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="4457a-104">Po vieną GAL automatiškai sukuriama kiekvienoje organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="4457a-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="4457a-105">Galite sukurti papildomų GAL atskiriems vartotojams pagal organizaciją arba vietą, bet vienas vartotojas gali matyti ir naudoti tik vieną GAL vienu metu.</span><span class="sxs-lookup"><span data-stu-id="4457a-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="4457a-106">Kai kurie el. pašto klientai, pvz., „Outlook, skirta „Windows“, atsisiunčia GAL, kad galėtumėte naudoti neprisijungę.</span><span class="sxs-lookup"><span data-stu-id="4457a-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="4457a-107">Tai vadinama autonomine adresų knygelė (OAB).</span><span class="sxs-lookup"><span data-stu-id="4457a-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="4457a-108">„Exchange Online“ OAB atnaujinamas tik kartą per 8 valandas, tada klientai turi atsisiųsti ir atnaujinti savo vietinę OAB kopiją.</span><span class="sxs-lookup"><span data-stu-id="4457a-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="4457a-109">Bet koks gavėjo keitimas pirmiausia turi būti matomas GAL, kad vėliau jis būtų OAB.</span><span class="sxs-lookup"><span data-stu-id="4457a-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="4457a-110">Štai keletas dažniausiai naudojamų GAL ir OAB procedūrų:</span><span class="sxs-lookup"><span data-stu-id="4457a-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="4457a-111">Dėl įvairių priežasčių galite norėti paslėpti objektus, kad jų nebūtų GAL.</span><span class="sxs-lookup"><span data-stu-id="4457a-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="4457a-112">Žr. [Gavėjų nerodymas adresų sąrašuose](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="4457a-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="4457a-113">Jei reikia suteikti konkrečioms vartotojų grupėms pritaikytus organizacijos GAL rodinius, ​​žr. [Adresų knygelės strategijos „Exchange Online“](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="4457a-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="4457a-114">[Kaip sukurti visuotinį adresų sąrašą „Exchange Online“](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) ir išmokti dirbti su GAL teisėmis, žr. [„Exchange Online“ adresų sąrašai](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="4457a-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="4457a-115">Atminkite, kad sukūrus naujus GAL, taip pat gali reikėti sukurti naują OAB.</span><span class="sxs-lookup"><span data-stu-id="4457a-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="4457a-116">Žr. [Autonominės adresų knygelės procedūros](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="4457a-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
