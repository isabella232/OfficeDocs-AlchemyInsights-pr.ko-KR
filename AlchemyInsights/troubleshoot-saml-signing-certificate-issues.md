---
title: SAML 서명 인증서 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529275"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="d7786-102">SAML 서명 인증서 문제 해결</span><span class="sxs-lookup"><span data-stu-id="d7786-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="d7786-103">SAML 서명 인증서 문제를 해결하려면 다음 권장 단계를 수행하세요.</span><span class="sxs-lookup"><span data-stu-id="d7786-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="d7786-104">SSO를 지원하는 엔터프라이즈 애플리케이션을 추가할 경우 Azure가 [SAML 서명 인증서](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)라는 인증서를 생성합니다.</span><span class="sxs-lookup"><span data-stu-id="d7786-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="d7786-105">이 인증서의 유효기간은 3년입니다.</span><span class="sxs-lookup"><span data-stu-id="d7786-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="d7786-106">인증서 만료 날짜를 변경하려면 [페더레이션 인증서의 만료 날짜를 사용자 지정하고 새 인증서에 롤오버](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d7786-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="d7786-107">Azure는 이 인증서를 사용하여 응용 프로그램에서 요청한 SAML 토큰에 서명하고 성공적인 SSO를 위해 이 토큰을 응용 프로그램으로 전송합니다.</span><span class="sxs-lookup"><span data-stu-id="d7786-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="d7786-108">이 작업을 완료하려면 Azure 포털에서 인증서를 다운로드한 후 애플리케이션 공급업체로 전송하여 SSO 프로세스를 완료하세요.</span><span class="sxs-lookup"><span data-stu-id="d7786-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="d7786-109">이 프로세스가 완료되면 응용 프로그램이 이 인증서를 신뢰하고 이 인증서로 서명된 모든 SAML 토큰이 응용 프로그램에서 승인됩니다.</span><span class="sxs-lookup"><span data-stu-id="d7786-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="d7786-110">이 인증서가 만료되면 새 인증서를 만들고 응용 프로그램 공급업체로 업데이트한 다음 Azure 측에서 활성화하세요.</span><span class="sxs-lookup"><span data-stu-id="d7786-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="d7786-111">자세한 내용은 [곧 만료되는 인증서 갱신](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d7786-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="d7786-112">인증서가 만료될 경우, 사용자는 차단되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d7786-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="d7786-113">현재 인증서가 만료되기 전에 수신될 [알림에 대한 전자 메일 주소를 추가](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration)합니다.</span><span class="sxs-lookup"><span data-stu-id="d7786-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="d7786-114">4단계는 선택 사항입니다.</span><span class="sxs-lookup"><span data-stu-id="d7786-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="d7786-115">응용 프로그램의 SAML 인증서 서명 옵션 및 인증서 서명 알고리즘을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="d7786-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="d7786-116">자세한 내용은 [인증서 서명 옵션 및 서명 알고리즘 변경](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d7786-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

