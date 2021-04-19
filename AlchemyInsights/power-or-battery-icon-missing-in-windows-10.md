---
title: "\"Windows 10\" trūksta maitinimo arba akumuliatoriaus piktogramos"
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790556"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="aa760-102">"Windows 10" trūksta maitinimo arba akumuliatoriaus piktogramos</span><span class="sxs-lookup"><span data-stu-id="aa760-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="aa760-103">Jei jūsų "Windows 10" įrenginyje yra akumuliatorius (pvz., nešiojamasis kompiuteris arba planšetinis kompiuteris arba kompiuteris, prijungtas per USB prie UPS), paprastai šalia laikrodžio užduočių juostoje rodoma maitinimo / akumuliatoriaus piktograma, pvz.:</span><span class="sxs-lookup"><span data-stu-id="aa760-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Akumuliatoriaus piktograma](media/battery-icon.png)

<span data-ttu-id="aa760-105">Jei nematote šios piktogramos, ji gali būti paslėpta:</span><span class="sxs-lookup"><span data-stu-id="aa760-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="aa760-106">Eikite **[į Parametrų > personalizavimas > užduočių juostoje](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="aa760-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="aa760-107">Srityje Pranešimai spustelėkite Pasirinkti, **kurios piktogramos rodomos užduočių juostoje.**</span><span class="sxs-lookup"><span data-stu-id="aa760-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="aa760-108">Tada sąraše **raskite "Power"** elementą ir perjunkite jo parametrą į **Įjungti**.</span><span class="sxs-lookup"><span data-stu-id="aa760-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Rodyti maitinimo piktogramą užduočių juostoje](media/power-icon-on.png)

<span data-ttu-id="aa760-110">**Trikčių diagnostika**</span><span class="sxs-lookup"><span data-stu-id="aa760-110">**Troubleshooting**</span></span>

<span data-ttu-id="aa760-111">Jei vadovavote anksčiau pateiktoms instrukcijoms ir **"Power"** perjungimas yra pilkas arba nematomas,  užduočių juostos ieškos lauke įveskite **įrenginių** tvarkytuvė , tada rezultatų sąraše pasirinkite Įrenginių tvarkytuvė.</span><span class="sxs-lookup"><span data-stu-id="aa760-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="aa760-112">Dalyje **Akumuliatoriai** dešiniuoju pelės mygtuku spustelėkite įrenginio akumuliatorių, spustelėkite **Išjungti**, tada spustelėkite **Taip**.</span><span class="sxs-lookup"><span data-stu-id="aa760-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="aa760-113">Palaukite kelias sekundes, tada dešiniuoju pelės mygtuku spustelėkite akumuliatorių ir spustelėkite **Įgalinti**.</span><span class="sxs-lookup"><span data-stu-id="aa760-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="aa760-114">Tada iš naujo paleiskite įrenginį.</span><span class="sxs-lookup"><span data-stu-id="aa760-114">Then restart your device.</span></span>

<span data-ttu-id="aa760-115">Jei ėjote anksčiau pateiktas instrukcijas, bet akumuliatoriaus piktograma nerodoma užduočių juostoje, užduočių juostos  ieškos lauke įveskite **Užduočių** tvarkytuvas , tada rezultatų sąraše spustelėkite Užduočių tvarkytuvas.</span><span class="sxs-lookup"><span data-stu-id="aa760-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="aa760-116">Skirtuko Procesai **dalyje** Pavadinimas dešiniuoju **pelės** mygtuku spustelėkite Naršyklė **,** tada spustelėkite Paleisti iš **naujo.**</span><span class="sxs-lookup"><span data-stu-id="aa760-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
