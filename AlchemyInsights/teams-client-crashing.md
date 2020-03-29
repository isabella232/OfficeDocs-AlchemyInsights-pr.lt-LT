---
title: Genda „Teams“ klientas?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030680"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="80554-102">Genda „Teams“ klientas?</span><span class="sxs-lookup"><span data-stu-id="80554-102">Teams client crashing?</span></span>

<span data-ttu-id="80554-103">Jei jūsų „Teams“ klientas genda, bandykite atlikti šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="80554-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="80554-104">Jei naudojate „Teams“ kompiuterio taikomąją programą, [įsitikinkite, kad programa yra visiškai atnaujinta](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="80554-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="80554-105">Įsitikinkite, kad visi [„Office 365“ URL ir adresų diapazonai](https://docs.microsoft.com/microsoftteams/connectivity-issues) pasiekiami.</span><span class="sxs-lookup"><span data-stu-id="80554-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="80554-106">Prisijunkite naudodami savo administratoriaus paskyrą ir patikrinkite [tarnybų sveikatos stebėjimo skydą](https://docs.microsoft.com/office365/enterprise/view-service-health), kad įsitikintumėte, jog nėra trikčių ar tarnybos veikimo pablogėjimo.</span><span class="sxs-lookup"><span data-stu-id="80554-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="80554-107">Paskutinis veiksmas, kurį galite atlikti – pabandyti išvalyti savo „Teams“ kliento talpyklą:</span><span class="sxs-lookup"><span data-stu-id="80554-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="80554-108">Visiškai išeikite iš „Microsoft Teams“ kompiuterio kliento.</span><span class="sxs-lookup"><span data-stu-id="80554-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="80554-109">Galite dešiniuoju pelės mygtuku spustelėti **„Teams“** piktogramų dėkle ir spustelėti **Uždaryti** arba galite paleisti užduočių tvarkytuvą ir visiškai nutraukti procesą.</span><span class="sxs-lookup"><span data-stu-id="80554-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="80554-110">Eikite į failų naršyklę ir įveskite %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="80554-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="80554-111">Būdami kataloge, matysite kelis iš šių aplankų:</span><span class="sxs-lookup"><span data-stu-id="80554-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="80554-112">Dalyje **Taikomosios programos talpykla** eikite į Talpykla ir panaikinkite visus failus talpyklos vietoje: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="80554-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="80554-113">Dalyje **Blob_storage** panaikinkite visus failus: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="80554-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="80554-114">Dalyje **Cache** panaikinkite visus failus: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="80554-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="80554-115">Dalyje **databases** panaikinkite visus failus: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="80554-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="80554-116">Dalyje **GPUCache** panaikinkite visus failus: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="80554-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="80554-117">Dalyje **IndexedDB** panaikinkite .db failą: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="80554-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="80554-118">Dalyje **Local Storage** panaikinkite visus failus: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="80554-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="80554-119">Galiausiai dalyje **tmp** panaikinkite bet kurį failą: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="80554-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="80554-120">Iš naujo paleiskite „Teams“ klientą.</span><span class="sxs-lookup"><span data-stu-id="80554-120">Restart your Teams client.</span></span>
