---
title: 2491 "테 넌 트 또는 사용자 재정의 ' 정책으로 인해 배달 된 피싱의 전자 메일 메시지
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728617"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="e34df-102">' 테 넌 트 또는 사용자 재정의 ' 정책으로 인해 배달 된 피싱에서 전자 메일 메시지 알림</span><span class="sxs-lookup"><span data-stu-id="e34df-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="e34df-103">"테 넌 트 또는 사용자 재정의로 인해 배달 되었습니다." 라는 기본 경고 정책이 Office 365 ATP P1 및 P2 라이선스가 있는 테 넌 트에 피싱.</span><span class="sxs-lookup"><span data-stu-id="e34df-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="e34df-104">이 경고가 나타나면 조사 해야 하는 단계는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="e34df-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="e34df-105">알림 메시지에서 **알림 보기** 를 클릭 하 여 보안 & 준수 센터의 **경고** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="e34df-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="e34df-106">**메시지 목록을 보거나** **탐색기에서 메시지를 보는**옵션을 보려면 경고를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e34df-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="e34df-107">이러한 옵션을 사용 하면 메시지 ID를 포함 하는 메시지의 세부 정보로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e34df-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="e34df-108">위협 탐색기 링크는 경고 조건과 일치 하는 메시지를 자동으로 필터링 합니다.</span><span class="sxs-lookup"><span data-stu-id="e34df-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="e34df-109">위협 탐색기에서 날짜 필터를 조정 해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e34df-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="e34df-110">수동으로 구성 된 재정의 때문에 피싱 메시지가 배달 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e34df-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="e34df-111">사용자가 허용 하는 보낸 사람 또는 도메인 집합입니다.</span><span class="sxs-lookup"><span data-stu-id="e34df-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="e34df-112">스팸 방지 정책에서 관리자가 허용 하는 보낸 사람 또는 도메인 집합입니다.</span><span class="sxs-lookup"><span data-stu-id="e34df-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="e34df-113">연결 필터 정책에서 허용 되는 IP 주소입니다.</span><span class="sxs-lookup"><span data-stu-id="e34df-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="e34df-114">에서 메시지를 허용 하도록 구성 된 메일 흐름 규칙 (전송 규칙이 라고도 함)</span><span class="sxs-lookup"><span data-stu-id="e34df-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="e34df-115">메시지가 피싱으로 잘못 표시 되었다고 생각 되 면 Outlook [보고서 메시지 추가 기능](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) 을 사용 하 여 Microsoft에 메시지 예제를 전송 합니다.</span><span class="sxs-lookup"><span data-stu-id="e34df-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
