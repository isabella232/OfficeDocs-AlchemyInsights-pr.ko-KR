---
title: Intune iOS에서 APNS 인증서 설정
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
- "9000654"
- "3543"
ms.openlocfilehash: 66590b8a063e74e80bbe3e1e497c596d63a54ece
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824045"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="b5505-102">Intune iOS에서 APNS 인증서 설정</span><span class="sxs-lookup"><span data-stu-id="b5505-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="b5505-103">Apple MDM Push 인증서(APNS(Apple Push Notification Service) 인증서라고도 함)가 구독에 구성되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="b5505-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="b5505-104">Apple MDM Push 인증서가 구성되지 않은 경우 iOS 및 MacOS 장치를 등록하고 관리할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b5505-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="b5505-105">Intune에 인증서를 추가한 후 사용자가 회사 포털 앱을 설치하여 iOS 장치를 등록할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b5505-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="b5505-106">Intune 테넌트에 APNS 인증서를 추가하는 단계별 지침을 보려면 다음 링크의 콘텐츠를 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="b5505-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="b5505-107">Apple MDM Push 인증서 받기</span><span class="sxs-lookup"><span data-stu-id="b5505-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="b5505-108">APN(Apple Push Notification 인증서)에 문제가 있는 경우 이 블로그 게시물: [Intune 및 APN 인증서: 질문과 대답 및 일반적인 문제](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b5505-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
