---
title: Single-Sign Azure Active Directory 가입 장치에 대한 설정
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403829"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="c9085-102">Azure Active Directory 가입 장치에 대한 Single Sign-On</span><span class="sxs-lookup"><span data-stu-id="c9085-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="c9085-103">사내 AD(Active Directory) 환경이 있는 경우 AD 도메인에 가입된 컴퓨터를 Azure AD에 가입하려는 경우 하이브리드 Azure AD 조인을 수행하여 이 작업을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9085-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="c9085-104">[방법: 하이브리드 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 조인 구현 계획은 사용자 환경에서 하이브리드 Azure AD 조인을 구현하는 관련 단계를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="c9085-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="c9085-105">비즈니스용 Windows Hello를 사용하여 Single-Sign Azure AD 가입 장치 구성</span><span class="sxs-lookup"><span data-stu-id="c9085-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="c9085-106">**PRT(기본 새로 고침 토큰) 문제** PRT(주 새로 고침 토큰)는 Windows 10, Windows Server 2016 이상 버전, iOS 및 Android 장치에서 Azure AD 인증의 주요 아티팩트입니다.</span><span class="sxs-lookup"><span data-stu-id="c9085-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="c9085-107">Microsoft 자사 토큰 브로커에 특수하게 발급된 JWT(JSON Web Token)으로, 이러한 장치에서 사용되는 응용 프로그램에서 SSO(Single Sign-On)를 사용하도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9085-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="c9085-108">[주 새로 고침 토큰이란?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)에서 Windows 10 장치에서 PRT를 발급, 사용 및 보호하는 방법에 대한 세부 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="c9085-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="c9085-109">**WamDefaultSet: YES 및 AzureADPrt: YES** 이러한 필드는 사용자가 디바이스에 로그인할 때 Azure AD에 인증을 완료한 것인지 여부를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="c9085-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="c9085-110">값이 **NO인** 경우 다음이 때문일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9085-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="c9085-111">등록 시 장치와 연결된 TPM의 잘못된 저장소 키입니다(상승된 실행 시 KeySignTest 확인).</span><span class="sxs-lookup"><span data-stu-id="c9085-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="c9085-112">대체 로그인 ID</span><span class="sxs-lookup"><span data-stu-id="c9085-112">Alternate Login ID</span></span>
- <span data-ttu-id="c9085-113">HTTP 프록시를 찾을 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="c9085-113">HTTP Proxy not found</span></span>

<span data-ttu-id="c9085-114">dsregcmd 명령 - [SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state) 상태를 사용하여 장치 문제 해결</span><span class="sxs-lookup"><span data-stu-id="c9085-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
