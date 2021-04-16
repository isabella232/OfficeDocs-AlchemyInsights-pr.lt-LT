---
title: Failas atidarytas tik skaityti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813192"
---
# <a name="file-open-read-only"></a><span data-ttu-id="89de0-102">Failas atidarytas tik skaityti</span><span class="sxs-lookup"><span data-stu-id="89de0-102">File open read-only</span></span>

<span data-ttu-id="89de0-103">Gali būti, kad atidarant failus jie atidaromi kaip skirti tik skaityti.</span><span class="sxs-lookup"><span data-stu-id="89de0-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="89de0-104">Kai kuriais atvejais tai yra papildoma sauga, pvz., kai atidarote failus iš interneto, ir kitais atvejais taip gali būti dėl parametro, kurį galima pakeisti.</span><span class="sxs-lookup"><span data-stu-id="89de0-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="89de0-105">Toliau pateikiami keli scenarijai, kai failas atidaro tik skaityti ir kai kuriuos veiksmus, kuriuos galite atlikti, kad jį pakeistų.</span><span class="sxs-lookup"><span data-stu-id="89de0-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="89de0-106">**Mano antivirusinė programa sukelia jų atidarymą tik skaityti**</span><span class="sxs-lookup"><span data-stu-id="89de0-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="89de0-107">Kai kurios antivirusinės programos gali apsaugoti jus nuo potencialiai nesaugių failų atidarydami juos tik skaityti.</span><span class="sxs-lookup"><span data-stu-id="89de0-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="89de0-108">Norint sužinoti, kaip koreguoti šiuos parametrus, gali tekti pasitikrinti antivirusinės programos teikėją.</span><span class="sxs-lookup"><span data-stu-id="89de0-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="89de0-109">Pvz., "BitDefender" turi turinį, kaip įtraukti taikomųjų programų išimtis čia: Kaip įtraukti taikomąją programą arba apdoroti [išimtis "Bitdefender" valdymo centre](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="89de0-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="89de0-110">**Ar failo ypatybės nustatytos kaip tik skaitomos?**</span><span class="sxs-lookup"><span data-stu-id="89de0-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="89de0-111">Failo ypatybes galite patikrinti dešiniuoju pelės mygtuku spustelėdami failą ir pasirinkdami Ypatybės.</span><span class="sxs-lookup"><span data-stu-id="89de0-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="89de0-112">Jei pažymėtas atributas Tik skaityti, galite jį panaikinti ir spustelėti Gerai.</span><span class="sxs-lookup"><span data-stu-id="89de0-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="89de0-113">**Turinys yra apsaugotame rodinyje**</span><span class="sxs-lookup"><span data-stu-id="89de0-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="89de0-114">Failuose iš interneto ir kitose potencialiai nesaugiose vietose gali būti virusų, kirminų ar kitų kenkėjiškų programų, galinčių pakenkti jūsų kompiuteriui.</span><span class="sxs-lookup"><span data-stu-id="89de0-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="89de0-115">Taip dažnai būna el. laiškų priedų arba atsisiųstų failų atveju.</span><span class="sxs-lookup"><span data-stu-id="89de0-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="89de0-116">Norint apsaugoti kompiuterį, failai iš šių potencialiai nesaugių vietų atidaromi apsaugotame rodinyje.</span><span class="sxs-lookup"><span data-stu-id="89de0-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="89de0-117">Naudodami apsaugotą rodinį, galite skaityti failą ir peržiūrėti jo turinį sumažindami riziką.</span><span class="sxs-lookup"><span data-stu-id="89de0-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="89de0-118">Daugiau informacijos apie apsaugotą rodinį ir parametrų keitimą žr. šiame straipsnyje: [Kas yra apsaugotas rodinys?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="89de0-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="89de0-119">**Ar "OneDrive" pilna?**</span><span class="sxs-lookup"><span data-stu-id="89de0-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="89de0-120">Jei failas saugomas "OneDrive", o jūsų "OneDrive" saugojimo vieta pilna, negalėsite įrašyti dokumento, kol nepateksite į jam skirtą vietą.</span><span class="sxs-lookup"><span data-stu-id="89de0-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="89de0-121">Galite patikrinti laisvos vietos "OneDrive" pranešimų centre spustelėdami "OneDrive" piktogramą ir pasirinkdami Tvarkyti saugyklą arba galite eiti į , prisijungti ir atkreipkite dėmesį, kiek vietos naudojama [https://onedrive.live.com](https://onedrive.live.com) apatiniame kairiajame ekrano kampe.</span><span class="sxs-lookup"><span data-stu-id="89de0-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="89de0-122">**Ar "Office" suaktyvintas?**</span><span class="sxs-lookup"><span data-stu-id="89de0-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="89de0-123">Jei "Office" nesuaktyvintas arba jei jūsų prenumeratos galiojimas baigėsi, gali būti, kad naudojate tik skaitymo sumažinto funkcionalumo režimą.</span><span class="sxs-lookup"><span data-stu-id="89de0-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="89de0-124">Informacijos, kaip aktyvinti "Office", žr.: [Nelicelicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="89de0-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="89de0-125">**Jei visa kita nepavyksta...**</span><span class="sxs-lookup"><span data-stu-id="89de0-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="89de0-126">Pabandykite iš naujo paleisti kompiuterį</span><span class="sxs-lookup"><span data-stu-id="89de0-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="89de0-127">"Office" naujinimų diegimas</span><span class="sxs-lookup"><span data-stu-id="89de0-127">Install Office updates</span></span>
    
- <span data-ttu-id="89de0-128">"Office" atkūrimas internete</span><span class="sxs-lookup"><span data-stu-id="89de0-128">Perform an Online repair of Office</span></span>
    

