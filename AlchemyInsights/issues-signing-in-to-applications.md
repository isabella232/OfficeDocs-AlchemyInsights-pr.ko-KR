---
title: 응용 프로그램 로그인 문제
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
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886903"
---
# <a name="issues-signing-in-to-applications"></a><span data-ttu-id="ed220-102">응용 프로그램 로그인 문제</span><span class="sxs-lookup"><span data-stu-id="ed220-102">Issues signing in to applications</span></span>

<span data-ttu-id="ed220-103">원인을 감지하거나 사용자 로그인 관련 문제를 진단하려면 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="ed220-103">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="ed220-104">[로그인 진단](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="ed220-104">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="ed220-105">사용자, 응용 프로그램, 로그인 시간, 요청 ID 또는 상관 관계 ID에 대한 세부 정보를 입력하여 분석할 이벤트를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="ed220-105">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="ed220-106">필요한 경우 변경하기 위해 수행할 수 있는 작업과 작업에 대한 세부 정보를 보여주는 진단 결과를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="ed220-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="ed220-107">다음은 응용 프로그램에 로그인할 때 발생할 수 있는 몇 가지 일반적인 문제입니다.</span><span class="sxs-lookup"><span data-stu-id="ed220-107">The following are some common issues you may experience when signing in to applications:</span></span>

1. <span data-ttu-id="ed220-108">사용자 또는 다른 사용자가 **Azure AD 로그인을 완료했지만 예기치 않은 메시지가 나타나는 경우** [응용 프로그램에 로그인할 때 예기치 않은 동의 프롬프트](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) 및 [응용 프로그램에 대한 동의를 수행할 때 예기치 않은 오류](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error) 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ed220-108">You or the user **has complete an Azure AD sign in, but are seeing an unexpected prompt** - See the articles [Unexpected consent prompt when signing in to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) and [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>
2. <span data-ttu-id="ed220-109">사용자 또는 다른 사용자가 **응용 프로그램에 직접 로그인했지만 사용자 포털 또는 액세스 패널의 딥 링크에서 응용 프로그램에 로그인할 수 없는 경우** [Azure AD 내 앱에서 응용 프로그램에 로그인하는 문제 해결](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="ed220-109">You or a user **has signed in to an application directly, but can't sign in to it from a deeplink on the custom portal or the access panel**: See [Troubleshoot problems signing in to an application from Azure AD My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).</span></span>
3. <span data-ttu-id="ed220-110">사용자 또는 다른 사용자가 **Azure AD 로그인을 완료했지만, 응용 프로그램에 오류 메시지가 표시되어 상요자가 로그인 흐름을 완료할 수 없는 경우** 문제는 앱이 Azure AD가 낸 응답을 수락하지 않았다는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="ed220-110">You or a user **has completed an Azure AD sign in, but the application displays an error message and doesn't let the user finish the sign-in flow**: The problem is that the app didn't accept the response that Azure AD issued.</span></span> <span data-ttu-id="ed220-111">문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error)를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="ed220-111">Follow [these steps](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) to troubleshoot.</span></span>
4. <span data-ttu-id="ed220-112">사용자 또는 다른 사용자가 **암호 Single Sign-On에 대해 구성된 비암호 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)의 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="ed220-112">You or a user **can’t sign in to a non-gallery application configured for password single sign-on**: Follow the guidance in [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) to troubleshoot.</span></span>
5. <span data-ttu-id="ed220-113">사용자 또는 다른 사용자가 **암호 Single Sign-On에 대해 구성된 Azure AD 암호 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)의 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="ed220-113">You or a user **can’t sign in to an Azure AD Gallery application configured for password single sign-on**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) to troubleshoot.</span></span>
6. <span data-ttu-id="ed220-114">사용자나 다른 사용자가 **Microsoft 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="ed220-114">You or a user **can't sign in to a Microsoft application**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) to troubleshoot.</span></span>
7. <span data-ttu-id="ed220-115">사용자 또는 다른 사용자가 **암호 Single Sign-On에 대해 구성된 비암호 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery)의 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="ed220-115">You or a user **can't sign in to a non-gallery application configured for federated single sign-on**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) to troubleshoot.</span></span>
8. <span data-ttu-id="ed220-116">사용자 또는 다른 사용자가 **암호 Single Sign-On에 대해 구성된 Azure AD 암호 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)의 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="ed220-116">You or a user **can't sign in to an Azure AD Gallery application configured for federated single sign-on**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) to troubleshoot.</span></span>
9. <span data-ttu-id="ed220-117">사용자나 다른 사용자가 **사용자가 개발한 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="ed220-117">You or a user **can't sign in to a custom-developed application**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) to troubleshoot.</span></span>
10. <span data-ttu-id="ed220-118">사용자 또는 다른 사용자가 **Azure AD 응용 프로그램 프록시를 사용하여 온-프레미스 응용 프로그램에 로그인할 수 없는 경우** 문제를 해결하려면 [다음 단계](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy)를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="ed220-118">You or a user **can't sign in to an on-premises application using the Azure AD application proxy**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) to troubleshoot.</span></span>

