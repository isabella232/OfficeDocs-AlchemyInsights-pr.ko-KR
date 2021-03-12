---
title: 조직의 전자 메일 메시지 검색 및 삭제하기
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737002"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="de03d-102">조직의 전자 메일 메시지 검색 및 삭제하기</span><span class="sxs-lookup"><span data-stu-id="de03d-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="de03d-103">다음 단계를 따릅니다:</span><span class="sxs-lookup"><span data-stu-id="de03d-103">Follow these steps:</span></span>

1. <span data-ttu-id="de03d-104">전역 관리자가 아닌 경우 계정을 **eDiscovery 관리자** 역할 그룹 또는 준수 검색 관리 역할에 추가해야 하는 메시지를 **검색합니다.**</span><span class="sxs-lookup"><span data-stu-id="de03d-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="de03d-105">메시지를 삭제하려면 조직 관리 역할 그룹  또는 검색 및 제거 관리 역할에 **가입해야 합니다.**</span><span class="sxs-lookup"><span data-stu-id="de03d-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="de03d-106">이러한 역할에 대한 사용 권한은 보안 및 준수 & [할당됩니다.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="de03d-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="de03d-107">[삭제할 메시지를 찾는](https://docs.microsoft.com/office365/securitycompliance/content-search) 콘텐츠 검색을 생성합니다.</span><span class="sxs-lookup"><span data-stu-id="de03d-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="de03d-108">[보안 및 준수 센터 PowerShell에 연결](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)합니다.</span><span class="sxs-lookup"><span data-stu-id="de03d-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="de03d-109">MFA를 사용하는 경우 다음 지침을 참조하세요. 다단계 인증을 & 보안 및 준수 [센터 PowerShell에 연결](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="de03d-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="de03d-110">메시지 삭제: `New-ComplianceSearchAction` cmdlet을 실행하여 메시지를 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="de03d-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="de03d-111">삭제된 메시지는 사용자의 복구 가능한 항목 폴더로 이동됩니다.</span><span class="sxs-lookup"><span data-stu-id="de03d-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="de03d-112">명령의 예는 [3단계: 메시지 삭제를 참조합니다.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="de03d-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
