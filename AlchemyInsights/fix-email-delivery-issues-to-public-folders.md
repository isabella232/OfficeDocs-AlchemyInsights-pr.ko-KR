---
title: 메일 사용이 가능한 공용 폴더에 대 한 전자 메일 배달 문제 해결
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366470"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="04bbd-102">메일 사용이 가능한 공용 폴더에 대 한 전자 메일 배달 문제 해결</span><span class="sxs-lookup"><span data-stu-id="04bbd-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="04bbd-103">외부 보낸 사람이 메일 사용이 가능한 공용 폴더에 메시지를 보낼 수 없고 보낸 사람에 게 오류가 발생 하는 경우 **(550 5.4.1)**, 공용 폴더에 대 한 전자 메일 도메인이 신뢰할 수 있는 도메인이 아닌 내부 릴레이 도메인으로 구성 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="04bbd-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="04bbd-104">[EAC (Exchange 관리 센터)](https://docs.microsoft.com/Exchange/exchange-admin-center)를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="04bbd-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="04bbd-105">**메일 흐름** \> **허용 도메인**으로 이동 하 여 허용 도메인을 선택한 다음 **편집**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="04bbd-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="04bbd-106">해당 도메인 유형이 **신뢰할**수 있는 것으로 설정 된 경우 열리는 속성 페이지에서 해당 값을 **내부 릴레이로** 변경 하 고 **저장**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="04bbd-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="04bbd-107">외부 보낸 사람에 **게 사용 권한이 없는 오류 (550 5.7.13)** 가 수신 되는 경우 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) 에서 다음 명령을 실행 하 여 공용 폴더의 익명 사용자에 대 한 사용 권한을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="04bbd-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="04bbd-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` 예를 들면 `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` 입니다.</span><span class="sxs-lookup"><span data-stu-id="04bbd-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="04bbd-109">외부 사용자가이 공용 폴더에 전자 메일을 보낼 수 있도록 하려면 사용자 익명에 CreateItems 액세스 권한을 추가 합니다.</span><span class="sxs-lookup"><span data-stu-id="04bbd-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="04bbd-110">예를 들면 `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`와 같습니다.</span><span class="sxs-lookup"><span data-stu-id="04bbd-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
