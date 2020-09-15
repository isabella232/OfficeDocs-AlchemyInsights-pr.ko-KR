---
title: 드라이브를 SharePoint에 매핑하면 액세스 거부 됨
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668749"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="ec0cc-102">네트워크 드라이브에 매핑된 SharePoint 라이브러리 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ec0cc-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="ec0cc-103">매핑된 네트워크 드라이브로 이동 하면 다음 메시지 중 하나가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ec0cc-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="ec0cc-104">**\\경로에 액세스할 수 없습니다. 이 네트워크 리소스를 사용할 수 있는 권한이 없을 수 있습니다. 이 서버의 관리자에 게 문의 하 여 액세스 권한이 있는지 확인 하십시오.**</span><span class="sxs-lookup"><span data-stu-id="ec0cc-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="ec0cc-105">**액세스가 거부 되었습니다. 이 위치에서 파일을 열기 전에 먼저 웹 사이트를 신뢰할 수 있는 사이트 목록에 추가 하 고 웹 사이트로 이동한 후 자동으로 로그인 하는 옵션을 선택 해야 합니다.**</span><span class="sxs-lookup"><span data-stu-id="ec0cc-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="ec0cc-106">[매핑된 네트워크 드라이브 문제 해결](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)에 대 한 도움말을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec0cc-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="ec0cc-107">라이브러리를 네트워크 드라이브로 매핑하는 기능은 일시적 이며 Internet Explorer 에서만 지원 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ec0cc-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="ec0cc-108">대신, [주문형 파일](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)을 포함 하는 [새 OneDrive 동기화 클라이언트와 SharePoint 파일을 동기화](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) 합니다.</span><span class="sxs-lookup"><span data-stu-id="ec0cc-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="ec0cc-109">로컬 저장소 공간을 사용하지 않고 OneDrive에서 모든 파일에 액세스합니다.</span><span class="sxs-lookup"><span data-stu-id="ec0cc-109">Access all your files in OneDrive without using local storage space.</span></span>
  