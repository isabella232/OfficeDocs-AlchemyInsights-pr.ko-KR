---
title: 온-프레미스용 원활한 SSO(Single Sign-On) 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753446"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="ecb16-102">온-프레미스용 원활한 SSO(Single Sign-On) 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ecb16-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="ecb16-103">원활한 SSO(Single Sign-On) 문제를 해결하려면 다음 단계를 수행하세요.</span><span class="sxs-lookup"><span data-stu-id="ecb16-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="ecb16-104">**AZUREADSSO 컴퓨터 계정의 Kerberos 암호 해독 키를 배포하려면 어떻게 하나요?**</span><span class="sxs-lookup"><span data-stu-id="ecb16-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="ecb16-105">최소 30일마다 Kerberos 암호 해독 키를 배포하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="ecb16-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="ecb16-106">이 작업을 수동으로 수행하려면 다음 [Kerberos 암호 해독 키를 롤아웃하는 방법](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ecb16-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="ecb16-107">**원활한 SSO 구성**</span><span class="sxs-lookup"><span data-stu-id="ecb16-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="ecb16-108">원활한 SSO를 배포하려면 [Azure Active Directory 원활한 Single Sign-On: 빠른 시작](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)의 단계를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="ecb16-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="ecb16-109">**권고**</span><span class="sxs-lookup"><span data-stu-id="ecb16-109">**Advisory**</span></span>

- <span data-ttu-id="ecb16-110">[Azure Active Directory 원활한 Single Sign-On: 질문과 대답](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - 이 문서에서는 Azure Active Directory 원활한 Single Sign-On(원활한 SSO)에 대한 질문과 대답을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ecb16-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="ecb16-111">새로운 콘텐츠가 있는지 지속적으로 다시 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="ecb16-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="ecb16-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - 원활한 SSO에 대한 기능 요청이나 기술적 질문을 하는 방법에 대한 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ecb16-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="ecb16-113">**문제 해결**</span><span class="sxs-lookup"><span data-stu-id="ecb16-113">**Troubleshoot**</span></span>

<span data-ttu-id="ecb16-114">[Azure Active Directory 원활한 Single Sign-On 문제 해결](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - 이 문서는 Azure AD(Azure Active Directory) 원환할 SSO(Single Sign-On) 관련 일반적인 문제에 대한 문제 해결 정보를 찾는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="ecb16-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







