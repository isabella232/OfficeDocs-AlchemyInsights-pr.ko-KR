---
title: PowerShell의 셀프 서비스 구매
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
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739976"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="b1595-102">PowerShell의 셀프 서비스 구매</span><span class="sxs-lookup"><span data-stu-id="b1595-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="b1595-103">MSCommerce PowerShell 모듈을 사용 하려면 TLS 1.2 (로컬 관리자 권한 필요)을 사용 하 여 Windows 10 장치에 설치 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1595-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="b1595-104">MSCommerce 모듈을 가져오고 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1595-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="b1595-105">로그인 하 라는 메시지가 표시 되 면 전역 또는 청구 관리자 역할 자격 증명을 사용 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1595-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="b1595-106">TLS 1.2이 없는 경우 정책을 가져오거나 업데이트 하려고 할 때 다음 오류가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1595-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="b1595-107">*ErrorMessage-기본 연결이 닫혔습니다. 보내기에서 예기치 않은 오류가 발생 했습니다.*</span><span class="sxs-lookup"><span data-stu-id="b1595-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



