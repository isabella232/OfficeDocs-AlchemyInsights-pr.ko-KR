---
title: 전자 필기장 열기 문제 해결
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002359"
- "4718"
ms.openlocfilehash: b7628cdbb7cd3bc60b97339cb59854fc73f0139e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744776"
---
# <a name="fix-issues-with-opening-notebooks"></a><span data-ttu-id="d08a2-102">전자 필기장 열기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="d08a2-102">Fix issues with opening notebooks</span></span>

<span data-ttu-id="d08a2-103">**중요**"Microsoft Teams에서 OneNote에 대한 제한 사항이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d08a2-103">**Important**: You may see the message, "We're experiencing limitations with OneNote in Microsoft Teams.</span></span> <span data-ttu-id="d08a2-104">웹용 OneNote를 사용하여 이 전자 필기장을 편집하세요.”라는 메시지가 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d08a2-104">Please use OneNote for the web to edit this notebook."</span></span>

<span data-ttu-id="d08a2-105">[메시지 센터 ID: 207439 - Microsoft 365 임시 기능 조정의 인식](https://admin.microsoft.com/Adminportal/Home?source=applauncher#MessageCenter?id=MC207439)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d08a2-105">Refer to [Message Center ID: 207439 - Awareness of Microsoft 365 temporary feature adjustments](https://admin.microsoft.com/Adminportal/Home?source=applauncher#MessageCenter?id=MC207439).</span></span>

<span data-ttu-id="d08a2-106">Teams의 OneNote는 상업용 및 교육용 테넌트에 대해 읽기 전용입니다.</span><span class="sxs-lookup"><span data-stu-id="d08a2-106">OneNote in Teams will be read-only for commercial and education tenants.</span></span> <span data-ttu-id="d08a2-107">편집하려면 웹용 OneNote 데스크톱 또는 OneNote 데스크톱 앱을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="d08a2-107">To edit, please use OneNote for the web or the OneNote desktop app.</span></span>

<span data-ttu-id="d08a2-108">다음은 전자 필기장 열기 문제에 대한 일반적인 몇 가지 해결 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="d08a2-108">Here are some common resolutions to issues with opening notebooks:</span></span>

1. <span data-ttu-id="d08a2-109">회사 또는 학교 계정이 아닌 개인 계정으로 로그인했기 때문에 전자 필기장을 열지못하고 있을 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d08a2-109">You may not be able to open the notebook because you are logged in with your personal account instead of your work or school account.</span></span>
    - <span data-ttu-id="d08a2-110">웹용 OneNote에서 전자 필기장이 열리는 경우, OneNote에서 현재 자격 증명으로 로그인하고 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="d08a2-110">If the notebook opens on OneNote for the web, make sure you are logging in with current credentials in OneNote.</span></span>
    - <span data-ttu-id="d08a2-111">OneNote 2016에서 **파일 > 계정**을 클릭하고 모든 계정에서 **로그아웃**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="d08a2-111">In OneNote 2016, click **File > Account** and **Sign Out** of all accounts.</span></span> <span data-ttu-id="d08a2-112">유효한 라이선스가 있는 사용자 계정을 사용하여 다시 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="d08a2-112">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="d08a2-113">자세한 내용은 [Office의 계정](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d08a2-113">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span> 
    - <span data-ttu-id="d08a2-114">Windows용 OneNote에서 화면 오른쪽 위에 있는 줄임표(**...**)를 클릭하고 **설정 > 계정**을 클릭한 다음, 회사 또는 학교 계정이 나열되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="d08a2-114">In OneNote for Windows, click the ellipsis (**…**) at the top right of the screen, click **Settings > Accounts**, and ensure that a work or school account is listed.</span></span> 
2. <span data-ttu-id="d08a2-115">열리지 않는 전자 필기장이 OneDrive 또는 SharePoint Online에 저장되어 있는 경우, [웹용 OneNote](https://onenote.com)에서 전자 필기장을 열어보세요.</span><span class="sxs-lookup"><span data-stu-id="d08a2-115">If the notebook that won't open is stored on OneDrive or SharePoint Online, try opening the notebook in [OneNote for the web](https://onenote.com).</span></span> <span data-ttu-id="d08a2-116">전자 필기장이 나열되지 않으면 전자 필기장에 대한 사용 권한이 없을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d08a2-116">If the notebook is not listed, you may not have permissions to it.</span></span> <span data-ttu-id="d08a2-117">공유 전자 필기장인 경우. 소유자에게 공유를 요청하고 올바른 계정을 사용하여 로그인하고 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="d08a2-117">If it is a shared notebook, ask the owner to share it and ensure that you are using the correct account to log in.</span></span>
