---
title: „Atidaryti naudojant „Explorer“ problemų šalinimas naudojant „SharePoint Online“
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 52429314d1529d0d2df7886feaebbcfd27666a06
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559705"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="26ba8-102">„Atidaryti naudojant „Explorer“ problemų šalinimas naudojant „SharePoint Online“</span><span class="sxs-lookup"><span data-stu-id="26ba8-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="26ba8-103">Komanda Atidaryti naudojant „Explorer“ atidaro vietinį „Windows Explorer“ egzempliorių, kuriame rodoma aplanko struktūra serveryje, kuriame yra „SharePoint“ svetainė.</span><span class="sxs-lookup"><span data-stu-id="26ba8-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="26ba8-104">Atsižvelgdami į tai, rekomenduojame [sinchronizuoti „SharePoint“ failus su naujuoju „OneDrive“ sinchronizavimo klientu](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, kuris teikia [failus pagal pareikalavimą](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), nes jis suteikia vietinę prieigą prie jūsų failų ir siūlo geriausią našumą.</span><span class="sxs-lookup"><span data-stu-id="26ba8-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="26ba8-105">Jei pasirinkote naudoti „Explorer“ rodinį, o ne naująjį „OneDrive“ sinchronizavimo klientą, būtinai atlikite toliau pateiktuose straipsniuose nurodytus veiksmus ir naudokitės ten aprašytais geriausios praktikos pavyzdžiais:</span><span class="sxs-lookup"><span data-stu-id="26ba8-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="26ba8-106">Kaip naudoti komandą „Atidaryti naudojant „Explorer“, norint išspręsti „SharePoint Online“ triktis</span><span class="sxs-lookup"><span data-stu-id="26ba8-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="26ba8-107">Bibliotekos failų kopijavimas arba perkėlimas naudojant parinktį Atidaryti naudojant „Explorer“</span><span class="sxs-lookup"><span data-stu-id="26ba8-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="26ba8-108">Mygtukas **Atidaryti naudojant „Explorer“** nerodomas naujojoje bibliotekos sąsajoje.</span><span class="sxs-lookup"><span data-stu-id="26ba8-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="26ba8-109">Viršutiniame dešiniajame kampe spustelėkite išplečiamąjį sąrašą **Rodinys** (išplečiamojo sąrašo pavadinimas keičiasi, atsižvelgiant į dabartinį rodinį), tada failų naršyklėje spustelėkite **Peržiūrėti failų naršyklėje**.</span><span class="sxs-lookup"><span data-stu-id="26ba8-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="26ba8-110">„SharePoint“ komanda Atidaryti naudojant „Explorer“ naudoja „ActiveX“ valdiklius, todėl ji palaikoma tik „Internet Explorer“ 10 arba 11 versijoje.</span><span class="sxs-lookup"><span data-stu-id="26ba8-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="26ba8-111">Komanda Atidaryti naudojant „Explorer“ neveikia sistemoje „Windows“ su „Microsoft Edge“, „Google Chrome“ ir „Mozilla Firefox“ arba „Mac“ platformoje.</span><span class="sxs-lookup"><span data-stu-id="26ba8-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="26ba8-112">Dėl šios priežasties „Explorer“ rodinio parinktis gali būti papilkinta.</span><span class="sxs-lookup"><span data-stu-id="26ba8-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="26ba8-113">[Kodėl „SharePoint“ juostelės mygtukai nepasiekiami arba papilkinti](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="26ba8-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

