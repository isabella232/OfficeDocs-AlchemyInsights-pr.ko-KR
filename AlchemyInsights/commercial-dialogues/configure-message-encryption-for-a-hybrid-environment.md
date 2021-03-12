---
title: 하이브리드 환경에 대한 메시지 암호화 구성
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736415"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="65889-102">하이브리드 환경에 대한 메시지 암호화 구성</span><span class="sxs-lookup"><span data-stu-id="65889-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="65889-103">하이브리드 Exchange 환경의 경우, 전자 메일이 Exchange Online을 통해 라우팅된 경우만 OME(Office 메시지 암호화)를 사용하여 암호화된 전자 메일을 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65889-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="65889-104">OME를 사용하여 전자 메일을 암호화하기 위해 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="65889-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="65889-105">하이브리드 [구성 마법사를 사용하여](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) 하이브리드 환경을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65889-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="65889-106">암호화를 설정하는 데 특별한 단계는 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="65889-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="65889-107">[평소처럼 암호화에](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) 대한 메일 흐름 규칙을 설정하세요.</span><span class="sxs-lookup"><span data-stu-id="65889-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


