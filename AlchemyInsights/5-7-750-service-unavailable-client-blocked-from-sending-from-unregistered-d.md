---
title: 1048 5.7.750 서비스를 사용할 수 없습니다. 등록되지 않은 도메인에서 전송이 차단된 클라이언트
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774257"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="a405e-103">5.7.750 클라이언트가 등록되지 않은 도메인에서의 전송을 차단함</span><span class="sxs-lookup"><span data-stu-id="a405e-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="a405e-104">이 오류는 테넌트에 프로비전되지 않은 도메인(허용 도메인으로 추가 및 유효성 검사)에서 대량의 메시지를 보낼 때 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="a405e-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="a405e-105">이 오류를 방지하려면 인증서의 도메인이 프로비전된 도메인인 인증서 기반 메일 흐름 커넥터를 사용하거나 모든 보내는 도메인을 프로비전할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a405e-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="a405e-106">자세한 내용은 [Exchange Online에서 오류 코드 5.7.700 ~ 5.7.750에 해당하는 전자 메일 배달 문제 수정](https://go.microsoft.com/fwlink/?linkid=2164955)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a405e-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>