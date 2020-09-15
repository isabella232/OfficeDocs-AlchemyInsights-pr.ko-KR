---
title: 최신 사이트를 루트 사이트로
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666876"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="69fb8-102">최신 사이트를 루트 사이트로</span><span class="sxs-lookup"><span data-stu-id="69fb8-102">Modern site as root site</span></span>

<span data-ttu-id="69fb8-103">Microsoft는 [클래식 사이트 루트 사이트를 최신 사이트로 바꾸는](https://docs.microsoft.com/sharepoint/modern-root-site)데 사용할 수 있는 새로운 기능을 배포 하기 시작 했습니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="69fb8-104">[SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 를 사용 하 여 원본 사이트를 보관 하는 동안 사이트의 위치를 다른 사이트와 교환 합니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="69fb8-105">두 팀 사이트 (그룹에 연결 되지 않음)와 통신 사이트에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="69fb8-106">최신 통신 사이트를 만들려면 클래식 루트 사이트를 삭제 하지 마십시오.</span><span class="sxs-lookup"><span data-stu-id="69fb8-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="69fb8-107">이 기능은 Microsoft에서 지원 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="69fb8-108">루트 사이트를 삭제 하면 사이트를 복원 하거나 같은 URL에 새 사이트를 만들 때까지 조직의 모든 SharePoint 사이트가 모든 사용자에 게 액세스 하지 못하게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="69fb8-109">메시지 센터를 통해이 기능을 전달 합니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="69fb8-110">잠시 후 테 넌 트에서 기능을 사용 하도록 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="69fb8-111">사이트 교체에 대 한 알려진 문제</span><span class="sxs-lookup"><span data-stu-id="69fb8-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="69fb8-112">대상 사이트에서 짧은 시간 동안 "찾을 수 없음" (HTTP 404) 오류가 반환 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="69fb8-113">콘텐츠를 다시 크롤링 하 여 검색 인덱스를 업데이트 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="69fb8-114">여기에는 수동 단계가 필요 하지 않으므로이 작업이 자동으로 수행 됩니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="69fb8-115">"정적" 링크 (예: 파일 동기화 및 OneNote 파일)에 종속 된 모든 것을 수동으로 수정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="69fb8-116">Project Server 사이트가 여전히 올바르게 연결 되어 있는지 확인 하기 위해 프로젝트 서버 사이트의 유효성을 검사 해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69fb8-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
