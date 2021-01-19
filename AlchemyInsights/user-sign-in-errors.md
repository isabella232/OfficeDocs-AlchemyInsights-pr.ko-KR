---
title: 사용자 로그인 오류
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886827"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="f4861-102">사용자 로그인 오류</span><span class="sxs-lookup"><span data-stu-id="f4861-102">User sign-in errors</span></span>

<span data-ttu-id="f4861-103">**로그인 진단 문제 해결**</span><span class="sxs-lookup"><span data-stu-id="f4861-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="f4861-104">원인을 감지하거나 사용자 로그인 관련 문제를 진단하려면 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="f4861-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="f4861-105">[로그인 진단](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="f4861-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="f4861-106">사용자, 응용 프로그램, 로그인 시간, 요청 ID 또는 상관 관계 ID에 대한 세부 정보를 입력하여 분석할 이벤트를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="f4861-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="f4861-107">필요한 경우 변경하기 위해 수행할 수 있는 작업과 작업에 대한 세부 정보를 보여주는 진단 결과를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="f4861-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="f4861-108">**Azure AD(Azure Active Directory) STS(보안 토큰 서비스)에서 반환되는 AADS 오류 코드에 대한 정보를 찾고 계신가요?**</span><span class="sxs-lookup"><span data-stu-id="f4861-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="f4861-109">[이 문서](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)를 읽고 AADSTS 오류 설명, 수정 및 제안된 해결 방법을 찾는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f4861-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>