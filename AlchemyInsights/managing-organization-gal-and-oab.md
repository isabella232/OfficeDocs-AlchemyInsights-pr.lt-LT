---
title: Organizacijos visuotinio adresų sąrašo ir autonominės adresų knygelės valdymas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794840"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="41b9c-102">Organizacijos visuotinio adresų sąrašo (GAL) ir autonominės adresų knygelės valdymas (OAB)</span><span class="sxs-lookup"><span data-stu-id="41b9c-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="41b9c-103">Visuotinis adresų sąrašas (GAL) yra objektų, kuriuose įgalintas el. paštas, sąrašas (bet kokio tipo gavėjas, kuris gali gauti el. laišką) organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="41b9c-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="41b9c-104">Po vieną GAL automatiškai sukuriama kiekvienoje organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="41b9c-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="41b9c-105">Galite sukurti papildomų GAL atskiriems vartotojams pagal organizaciją arba vietą, bet vienas vartotojas gali matyti ir naudoti tik vieną GAL vienu metu.</span><span class="sxs-lookup"><span data-stu-id="41b9c-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="41b9c-106">Kai kurie el. pašto klientai, pvz., „Outlook, skirta „Windows“, atsisiunčia GAL, kad galėtumėte naudoti neprisijungę.</span><span class="sxs-lookup"><span data-stu-id="41b9c-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="41b9c-107">Tai vadinama autonomine adresų knygelė (OAB).</span><span class="sxs-lookup"><span data-stu-id="41b9c-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="41b9c-108">„Exchange Online“ OAB atnaujinamas tik kartą per 8 valandas, tada klientai turi atsisiųsti ir atnaujinti savo vietinę OAB kopiją.</span><span class="sxs-lookup"><span data-stu-id="41b9c-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="41b9c-109">Bet koks gavėjo keitimas pirmiausia turi būti matomas GAL, kad vėliau jis būtų OAB.</span><span class="sxs-lookup"><span data-stu-id="41b9c-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="41b9c-110">Štai keletas dažniausiai naudojamų GAL ir OAB procedūrų:</span><span class="sxs-lookup"><span data-stu-id="41b9c-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="41b9c-111">Dėl įvairių priežasčių galite norėti paslėpti objektus, kad jų nebūtų GAL.</span><span class="sxs-lookup"><span data-stu-id="41b9c-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="41b9c-112">Žr. [Gavėjų nerodymas adresų sąrašuose](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="41b9c-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="41b9c-113">Jei reikia suteikti konkrečioms vartotojų grupėms pritaikytus organizacijos GAL rodinius, ​​žr. [Adresų knygelės strategijos „Exchange Online“](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="41b9c-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="41b9c-114">[Kaip sukurti visuotinį adresų sąrašą „Exchange Online“](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) ir išmokti dirbti su GAL teisėmis, žr. [„Exchange Online“ adresų sąrašai](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="41b9c-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="41b9c-115">Atminkite, kad sukūrus naujus GAL, taip pat gali reikėti sukurti naują OAB.</span><span class="sxs-lookup"><span data-stu-id="41b9c-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="41b9c-116">Žr. [Autonominės adresų knygelės procedūros](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="41b9c-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
