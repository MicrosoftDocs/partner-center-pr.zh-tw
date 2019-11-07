---
title: 閱讀您的帳單 |合作夥伴中心
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 您的發票是目前每個月期間 (在程式、產品以及客戶) 的所有費用摘要。 可在合作夥伴中心取得。
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: 訂閱計費, 計費, 合作夥伴中心的計費, 合作夥伴中心計費, 閱讀帳單, 發票, 合作夥伴中心發票, CSP 發票, 我的帳單在哪裡？
ms.localizationpriority: medium
ms.openlocfilehash: 37469a72137d5bc399f5ab765c49c8accd36808d
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652178"
---
# <a name="read-your-bill"></a>閱讀您的帳單

**適用於**

-  合作夥伴中心
-  Microsoft Cloud for US Government 適用的合作夥伴中心


針對您的帳單，請移至 [**合作夥伴中心**] 功能表，然後選取 [**帳單**] 以查看您的帳單歷程記錄和趨勢、發票和對帳檔案的連結，以及您最近的付款。

如果雲端解決方案提供者計畫中的合作夥伴已選擇每月計費，應於 60 天內，向 Microsoft 支付其客戶的訂閱費用 (包括授權型與用量型)。

> [!NOTE]  
> 您的發票是所有費用的摘要--在方案、產品和客戶之間--適用于目前的計費期間，並可在所選計費日期的兩個（2）天內（以 UTC 時程表示）。 例如，如果您有9月12日計費日期，發票產生程式將從第13：上午 10:00 PST UTC 開始，並在第14個上完成12：上午 10:00 PST UTC。 如果您在15日沒有看到您的發票（59PM UTC），您就不在服務等級協定，應該提出服務要求。 

您會針對授權型 (Office365) 及用量型 (Azure) 費用收到一張發票，以及針對一次性 (Azure 保留的 VM 執行個體) 的費用收到另一張發票。

如需費用的分項詳細資料，請使用隨附的對帳檔案。 對帳檔案包含客戶識別碼和您將用來建立客戶發票的訂閱識別碼。 如需詳細資訊，請參閱[如何使用對帳檔案](use-the-reconciliation-files.md)。

## <a name="invoice-file-definitions"></a>發票檔案定義


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>欄位</strong></td>
<td><strong>描述</strong></td>
</tr>
<tr class="even">
<td>美國 FEIN</td>
<td>您的聯邦稅務識別碼。</td>
</tr>
<tr class="odd">
<td>客戶號碼</td>
<td>您的客戶號碼。</td>
</tr>
<tr class="even">
<td>帳單地址</td>
<td>我們可寄送發票給您的收件地址。 若要變更公司名稱或位址，請編輯您的合作夥伴中心帳單設定檔。 </td>
</tr>
<tr class="odd">
<td>授權型費用</td>
<td>所購買之用量型授權的每月 (或每年度) 的定額金額 (於服務前預先計費)。 這個數字是授權型對帳檔案 (欄位 T) 中，&quot;Subtotal&quot; 欄位中的所有費用總和。</td>
</tr>
<tr class="even">
<td>用量型費用</td>
<td>Azure 使用量，包括在帳單月份啟用和使用的新服務或應用程式。 這個數字是用量型對帳檔案 (欄位 Z) 中，&quot;PretaxCharges&quot; 欄位中的所有費用總和。</td>
</tr>
<tr class="odd">
<td>折扣</td>
<td>例如，客戶以一般訂閱價格訂閱時獲得的折扣。 這會顯示為定額金額，而不是每一單位或每一授權的價格。</td>
</tr>
<tr class="odd">
<td>點數</td>
<td>對訂閱所做之變更的額度或調整 (例如：增加或減少訂閱基座)。</td>
</tr>
<tr class="even">
<tr class="even">
<td>小計</td>
<td>稅前總計以及稅收專屬費用和點數。</td>
</tr>
<td>稅</td>
<td>在發票第 2 頁開始位置的詳細資料區段中加總的目前費用的總稅金。 此數字是以下所有費用的總和：
<ul>
<li>用量型對帳檔案 (欄位 AA) 的 &quot;TaxAmount&quot; 欄位，和</li>
<li>授權型檔案 (欄位 U) 的 &quot;Tax&quot; 欄位。</li>
</ul></td>
</tr>
<tr class="odd">
<td>其他點數</td>
<td>稅收專屬點數。</td>
</tr>
<tr class="even">
<td>目前總費用</td>
<td>付款期限到期時，以您使用的帳單貨幣計算的帳單期間應付金額。</td>
</tr>
<tr class="odd">
<td>付款指示</td>
<td>描述如何支付發票 (根據您的地區)。 付款時，一律包含您的發票號碼。</td>
</tr>
<tr class="even">
<td>發票號碼</td>
<td>發票的號碼。</td>
</tr>
<tr class="odd">
<td>計費期間</td>
<td>以發票日期為開頭的每月期間。 這是使用以使用量為基礎之服務的期間，而以授權為基礎的服務則會針對任何信用額度調整或授權計數的變更進行協調。</td>
</tr>
<tr class="even">
<td>發票日期</td>
<td>每個月產生發票的帳單日期或週年日。</td>
</tr>
<tr class="odd">
<td>付款期限</td>
<td>對於一次性購買，這一律是 60 天。</td>
</tr>
<tr class="even">
<td>付款截止日期</td>
<td>必須在此日期前收到您的付款。</td>
</tr>
<tr class="odd">
<td>客戶採購單</td>
<td>您的採購單號碼。</td>
</tr>
<tr class="even">
<td>客戶服務</td>
<td>存取客戶服務的網址。</td>
</tr>
<tr class="odd">
<td>服務收件者</td>
<td>服務使用所在的地址。 （這是與公司調查相關聯的合法公司位址）。</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>一次性費用的分項清單

|**欄位** |**定義**|
|:----------------|:-----------------------------|
|日期 |購買日期。 |
|說明 |產品名稱。 |
|數量 |購買的產品 (例如保留區) 數目。 |
|單價 |產品 (例如保留區) 的單價。 |
|折扣 |適用的任何折扣。 |
|稅前金額 |稅前購買小計。 |
|營業稅 |稅額。 |
|總計 |至今應付總額。 |
 



