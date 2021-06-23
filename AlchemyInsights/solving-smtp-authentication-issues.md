---
title: SMTP autentifikavimo ir trikčių diagnostikos įgalinimas
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077659"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="118db-102">SMTP autentifikavimo ir trikčių diagnostikos įgalinimas</span><span class="sxs-lookup"><span data-stu-id="118db-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="118db-103">Jei norite įgalinti pašto dėžutės SMTP autentifikavimą arba gaunate klaidą "Klientas nėra autentifikuotas", "Autentifikavimas nesėkmingas" arba "SmtpClientAuthentication" su kodu 5.7.57 arba 5.7.3 arba 5.7.139, kai bandote perduoti el. paštą autentifikuojant įrenginį arba taikomąją programą su "Microsoft 365", atlikite šiuos tris veiksmus, kad išspręstumėte problemą:</span><span class="sxs-lookup"><span data-stu-id="118db-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="118db-104">Išjunkite ["Azure" saugos numatytąsias](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) reikšmes, įjungdami **Įjungti saugos numatytąsias reikšmes į** **Ne**.</span><span class="sxs-lookup"><span data-stu-id="118db-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="118db-105">a.</span><span class="sxs-lookup"><span data-stu-id="118db-105">a.</span></span> <span data-ttu-id="118db-106">Prisijunkite prie "Azure" portalo kaip saugos administratorius, sąlyginės prieigos administratorius arba visuotinis administratorius.</span><span class="sxs-lookup"><span data-stu-id="118db-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="118db-107">b.</span><span class="sxs-lookup"><span data-stu-id="118db-107">b.</span></span> <span data-ttu-id="118db-108">Raskite "Azure Active Directory" > **Ypatybės**.</span><span class="sxs-lookup"><span data-stu-id="118db-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="118db-109">c.</span><span class="sxs-lookup"><span data-stu-id="118db-109">c.</span></span> <span data-ttu-id="118db-110">Pasirinkite **Valdyti saugos numatytąsias reikšmes**.</span><span class="sxs-lookup"><span data-stu-id="118db-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="118db-111">d.</span><span class="sxs-lookup"><span data-stu-id="118db-111">d.</span></span> <span data-ttu-id="118db-112">Nustatykite **Įjungti saugos numatytąsias reikšmes kaip** **Ne**.</span><span class="sxs-lookup"><span data-stu-id="118db-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="118db-113">e.</span><span class="sxs-lookup"><span data-stu-id="118db-113">e.</span></span> <span data-ttu-id="118db-114">Pasirinkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="118db-114">Select **Save**.</span></span>

2. <span data-ttu-id="118db-115">[Įgalinkite kliento SMTP pateikimą](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) licencijuotose pašto dėžutėse.</span><span class="sxs-lookup"><span data-stu-id="118db-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="118db-116">a.</span><span class="sxs-lookup"><span data-stu-id="118db-116">a.</span></span> <span data-ttu-id="118db-117">Iš "Microsoft 365" administravimo centras eikite į **Aktyvūs vartotojai** ir pasirinkite vartotoją.</span><span class="sxs-lookup"><span data-stu-id="118db-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="118db-118">b.</span><span class="sxs-lookup"><span data-stu-id="118db-118">b.</span></span> <span data-ttu-id="118db-119">Eikite į skirtuką Paštas ir dalyje **El. pašto programos** pasirinkite **Valdyti el. pašto programas**.</span><span class="sxs-lookup"><span data-stu-id="118db-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="118db-120">d.</span><span class="sxs-lookup"><span data-stu-id="118db-120">d.</span></span> <span data-ttu-id="118db-121">**Įsitikinkite, kad pažymėta Autentifikuota SMTP** (įjungta).</span><span class="sxs-lookup"><span data-stu-id="118db-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="118db-122">e.</span><span class="sxs-lookup"><span data-stu-id="118db-122">e.</span></span> <span data-ttu-id="118db-123">Pasirinkite **Įrašyti keitimus**.</span><span class="sxs-lookup"><span data-stu-id="118db-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="118db-124">[Išjunkite kelių dalių autentifikavimą (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) licencijuotose pašto dėžutėse.</span><span class="sxs-lookup"><span data-stu-id="118db-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="118db-125">a.</span><span class="sxs-lookup"><span data-stu-id="118db-125">a.</span></span> <span data-ttu-id="118db-126">Eikite į "Microsoft 365" administravimo centras ir kairiajame naršymo meniu pasirinkite Vartotojai  >  **aktyvūs vartotojai**.</span><span class="sxs-lookup"><span data-stu-id="118db-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="118db-127">b.</span><span class="sxs-lookup"><span data-stu-id="118db-127">b.</span></span> <span data-ttu-id="118db-128">Pasirinkite **Kelių dalių autentifikavimas**.</span><span class="sxs-lookup"><span data-stu-id="118db-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="118db-129">c.</span><span class="sxs-lookup"><span data-stu-id="118db-129">c.</span></span> <span data-ttu-id="118db-130">Pasirinkite vartotoją ir išjunkite **kelių dalių autentifikavimą**.</span><span class="sxs-lookup"><span data-stu-id="118db-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
