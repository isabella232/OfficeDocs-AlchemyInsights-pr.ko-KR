---
title: 전송 규칙을 사용하여 암호화
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784349"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="2de5c-102">전송 규칙을 사용하여 암호화</span><span class="sxs-lookup"><span data-stu-id="2de5c-102">Encryption with transport rules</span></span>

<span data-ttu-id="2de5c-103">[Exchange 관리 센터](https://go.microsoft.com/fwlink/p/?linkid=834822)(EAC)에서 메일 흐름 규칙의 Office 메시지 암호화(OME) 기능을 사용하여 메시지 암호화를 트리거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2de5c-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="2de5c-104">전송 규칙 조건에서 **Office 365 메시지 암호화 및 권한 보호 적용** 옵션을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="2de5c-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="2de5c-105">자세한 내용은 [암호화를 위한 메일 흐름 규칙 정의](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2de5c-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="2de5c-106">Powershell에서 [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet을 사용하고 매개 변수 *ApplyOME*를 $true로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="2de5c-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
