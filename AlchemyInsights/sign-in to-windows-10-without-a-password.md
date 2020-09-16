---
title: Prisijungimas prie "Windows 10" nenaudojant slaptažodžio
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719961"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="96be8-102">Prisijungimas prie "Windows 10" nenaudojant slaptažodžio</span><span class="sxs-lookup"><span data-stu-id="96be8-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="96be8-103">Kad nereikėtų įvesti slaptažodžio "Windows" paleisties metu, rekomenduojame naudoti vieną iš "Windows Hello" saugaus prisijungimo parinkčių, pvz., PIN, veido atpažinimo arba pirštų atspaudų, jei yra.</span><span class="sxs-lookup"><span data-stu-id="96be8-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="96be8-104">Jei tikrai norite išjungti saugią prisijungimo funkciją, peržiūrėkite toliau pateiktas instrukcijas "automatiškai prisijungti prie" Windows 10 ".</span><span class="sxs-lookup"><span data-stu-id="96be8-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="96be8-105">**Apsaugokite "Windows Hello" į paskyros slaptažodį**</span><span class="sxs-lookup"><span data-stu-id="96be8-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="96be8-106">Eikite į **parametrai > paskyros > prisijungimo parinktys** (arba spustelėkite [čia](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="96be8-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="96be8-107">Bus įtrauktos galimos prisijungimo parinktys.</span><span class="sxs-lookup"><span data-stu-id="96be8-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="96be8-108">Pavyzdžiui:</span><span class="sxs-lookup"><span data-stu-id="96be8-108">For example:</span></span>

![Prisijungimo parinktys.](media/sign-in-options.png)

<span data-ttu-id="96be8-110">Spustelėkite arba bakstelėkite vieną iš parinkčių, kad ją sukonfigūruotumėte.</span><span class="sxs-lookup"><span data-stu-id="96be8-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="96be8-111">Kai tik pradėsite arba atrakinsite "Windows", galėsite naudoti naują parinktį vietoj slaptažodžio.</span><span class="sxs-lookup"><span data-stu-id="96be8-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="96be8-112">**Automatinis prisijungimas prie "Windows 10"**</span><span class="sxs-lookup"><span data-stu-id="96be8-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="96be8-113">**Pastaba**: Automatinis prisijungimas yra patogus, tačiau įveda saugos pavojų, ypač, jei jūsų kompiuterį gali naudoti keli žmonės.</span><span class="sxs-lookup"><span data-stu-id="96be8-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="96be8-114">Spustelėkite arba bakstelėkite mygtuką **pradėti** užduočių juostoje.</span><span class="sxs-lookup"><span data-stu-id="96be8-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="96be8-115">Įveskite **netplwiz** ir paspauskite klavišą "įvesti", kad atidarytumėte langą vartotojų abonementai.</span><span class="sxs-lookup"><span data-stu-id="96be8-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="96be8-116">**Vartotojų abonementuose**spustelėkite abonementą, kurį norite automatiškai prisijungti, kai "Windows" pradės.</span><span class="sxs-lookup"><span data-stu-id="96be8-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="96be8-117">Atžymėkite žymimąjį langelį "vartotojai turi įvesti vartotojo vardą ir slaptažodį, kad galėtų naudoti šį kompiuterį".</span><span class="sxs-lookup"><span data-stu-id="96be8-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Vartotojai turi įvesti vartotojo vardą ir slaptažodį.](media/users-must-enter-username.png)

5. <span data-ttu-id="96be8-119">Spustelėkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="96be8-119">Click **OK**.</span></span> <span data-ttu-id="96be8-120">Jūsų bus paprašyta įvesti ir patvirtinti pasirinkto abonemento slaptažodį.</span><span class="sxs-lookup"><span data-stu-id="96be8-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="96be8-121">Spustelėkite **gerai** , kad pabaigtumėte.</span><span class="sxs-lookup"><span data-stu-id="96be8-121">Click **OK** to finish.</span></span> <span data-ttu-id="96be8-122">Paleidus "Windows 10", jis automatiškai prisijungs prie pasirinktos paskyros.</span><span class="sxs-lookup"><span data-stu-id="96be8-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
