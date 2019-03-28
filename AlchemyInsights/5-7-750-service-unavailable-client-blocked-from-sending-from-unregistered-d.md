---
title: 1048 5.7.750 서비스를 사용할 수 없습니다. 클라이언트가 등록 되지 않은 도메인에서 보내지 못하도록 차단 됨
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 5eb42679f123fcd1b680327329721cb47e18e11a
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776507"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="f77f3-103">등록 되지 않은 도메인에서 5.7.750 클라이언트의 송신이 차단 됨</span><span class="sxs-lookup"><span data-stu-id="f77f3-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="f77f3-104">이 오류는 많은 양의 메시지가 Office 365에서 프로 비전 되지 않은 도메인 (허용 도메인으로 추가 및 유효성 검사)으로 전송 될 때 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="f77f3-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>
  
<span data-ttu-id="f77f3-105">이 오류가 발생 하지 않도록 하려면 인증서의 도메인이 프로 비전 된 도메인인 인증서 기반 메일 흐름 커넥터를 사용 하거나 모든 보낸 도메인을 프로 비전 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f77f3-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
  
