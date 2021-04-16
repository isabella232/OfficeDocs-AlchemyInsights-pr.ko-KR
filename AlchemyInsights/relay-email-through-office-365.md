---
title: Microsoft 365를 통해 전자 메일 릴레이
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809661"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="09548-102">전자 메일을 보내도록 다기능 장치 또는 애플리케이션 설정</span><span class="sxs-lookup"><span data-stu-id="09548-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="09548-103">옵션 및 단계에 대한 자세한 내용은 [Microsoft 365를 사용하여 전자 메일을 보내도록 다기능 장치 또는 애플리케이션을 설정하는 방법](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="09548-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="09548-104">**참고:** 최근에 작동이 중지된 디바이스 또는 응용 프로그램이 있다면 최근 Microsoft가 예정대로 [3DES 암호화를 사용하지 않도록 설정](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption)하기 시작했다는 점을 알아두세요.</span><span class="sxs-lookup"><span data-stu-id="09548-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="09548-105">영향을 받는 장치를 보려면 [SMTP 인증 클라이언트 보고서](https://protection.office.com/mailflow/dashboard)로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="09548-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="09548-106">일반적인 오류는 인증 실패/오류, TLS 실패/오류, 암호화 알고리즘 오류, 알고리즘 불일치 또는 연결 끊김과 유사할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="09548-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="09548-107">이 문제를 해결하려면:</span><span class="sxs-lookup"><span data-stu-id="09548-107">To resolve the issue:</span></span>

 - <span data-ttu-id="09548-108">**Windows Server 2003 IIS SMTP가 더 이상 작동하지 않으며 Windows의 새 버전이 필요합니다.**</span><span class="sxs-lookup"><span data-stu-id="09548-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="09548-109">최신 암호화가 지원되는지 또는 업데이트가 있는지 알아보려면 응용 프로그램 또는 디바이스 공급업체를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="09548-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
