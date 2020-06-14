---
title: 基於使用方式的對帳檔案
ms.topic: article
ms.date: 06/08/2020
description: 瞭解您在合作夥伴中心內以使用量為基礎的對帳檔案中的所有專案。 包含幾個範例。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 83545002fbc0138e4020473a9554d9127e7771b4
ms.sourcegitcommit: 0154eabccdc92d1fbe73734f5514f317b9e9fee0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/12/2020
ms.locfileid: "84749211"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>瞭解以使用量為基礎的對帳檔案及其在合作夥伴中心的特定欄位

適用於：

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

若要根據客戶的使用量來協調您的費用，請將**ResellerID**、 **ResellerName**和**ResellerBillableAccount**與來自「合作夥伴中心」的**客戶名稱**和訂用帳戶**識別碼**進行比對。

## <a name="fields-in-usage-based-reconciliation-files"></a>以使用量為基礎的對帳檔案中的欄位

下列欄位說明使用哪些服務及費率。

| 資料行 | 描述 | 範例值 |
| ------ | ----------- | ------------ |
| PartnerId | 合作夥伴識別碼（GUID 格式）。 | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | 合作夥伴名稱。 | *Contoso，公司。* |
| PartnerBillableAccountId | 合作夥伴帳戶識別碼。 | *1010578050* |
| CustomerCompanyName | 客戶的組織名稱（如合作夥伴中心所報告）。 *將發票與您的系統資訊進行協調非常重要。* | *測試客戶* |
| MpnId | CSP 合作夥伴的 MPN 識別碼。 | *4390934* |
| ResellerMpnId | 訂用帳戶之記錄轉銷商的 MPN 識別碼。  |
| InvoiceNumber | 出現指定交易的發票號碼。 | *D020001IVK* |
| ChargeStartDate | 計費週期的開始日期，但在呈現先前不收費潛在使用量資料的日期 (來自先前帳單週期) 時除外。 此時間一律為第一天的開始時間，即 0:00。 | *2/1/2019 0:00* |
| ChargeEndDate | 計費週期的結束日期，但在呈現先前不收費潛在使用量資料的日期 (來自先前帳單週期) 時除外。 時間一律是一天的結束時間 (23:59)。 | *2/28/2019 23:59* |
| SubscriptionId | Microsoft 計費平台中訂用帳戶的唯一識別碼。 在聯絡支援人員時，識別訂用帳戶可能會很有用。 不用於對帳。 *這與合作夥伴系統管理員主控台上的訂用帳戶**識別碼**不同。* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | 服務供應專案的昵稱。 | *Microsoft Azure* |
| SubscriptionDescription | 服務供應項目的業務線。 | *Microsoft Azure* |
| OrderID | Microsoft 計費平台中訂單的唯一識別碼。 在聯絡支援人員時，識別訂用帳戶可能會很有用。 不用於對帳。 | *566890604832738111* |
| ServiceName | 要求的 Azure 服務名稱。 | *虛擬機器* |
| ServiceType | 特定類型的 Azure 服務。 | *服務匯流排-個人或套件*、 *SQL Azure 資料庫-Business 或 Web Edition* |
| ResourceGuid | 所有服務資料和定價結構的特定唯一識別碼。 | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Azure 資源的名稱。 | *資料傳輸（gb）*，*資料傳出（gb）* |
| 區域 | 套用使用量的區域。 主要用來指派資料傳輸的速率，因為費率因地區而異。 | *亞太地區*、*歐洲*、*拉丁美洲*、*北美洲* |
| SKU | 供應專案的唯一 Microsoft 識別碼。 | *7UD-00001* |
| DetailLineItemId | 在指定的計費期間內，針對服務或資源的不同費率進行分級的識別碼和數量。 針對 Azure 階層式定價，可能會有一個費率，最高可達特定數量的計費單位，然後在該數量之後有不同的費率。 | *1* |
| ConsumedQuantity | 報告期間所耗用的服務數量（例如小時或 GB）。 也包含先前報告期間中任何未計費的使用量。 | *11* |
| IncludedQuantity | 納入供應項目中的單位。 通常不會出現在 CSP 中。 | *0* |
| OverageQuantity | 不包含在供應專案中的單位。 合作夥伴必須支付這些費用。 等於**ConsumedQuantity**減**IncludedQuantity**。 | *11* |
| ListPrice | 優惠價格會在訂用帳戶的開始日期生效。 | *$0.0808* |
| PretaxCharges | 等於**ListPrist**乘以**OverageQuantity**，舍入到最接近的美分。 | *$0.085* |
| TaxAmount | 收取的稅金金額。 根據您市場的稅務規則和特定情況。 | *$0.08* |
| PostTaxTotal | 稅後總計 (若有適用稅賦)。 | *$0.93* |
| 貨幣 | 貨幣類型。 每個計費實體都只有一個貨幣。 檢查它是否符合您的第一張發票，然後再進行任何主要的計費平臺更新。 | *歐元* |
| PretaxEffectiveRate | 每單位的稅前價格。 等於**計算 pretaxcharges**除以**OverageQuantity**，四捨五入為最接近的美分。 | *$0.08* |
| PostTaxEffectiveRate | 每單位的稅後價格。 等於**PostTaxTotal**除以**OverageQuantity**，四捨五入為最接近的美分。 或者，等於**PretaxEffectiveRate**加上每單位金額的稅率，舍入到最接近的美分。 | *$0.08* |
| ChargeType | 費用或調整的[類型](recon-file-charge-types.md)。 | 請參閱[費用類型](recon-file-charge-types.md)。 |
| CustomerId | 客戶的唯一 Microsoft 識別碼（GUID 格式）。 | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | 客戶的功能變數名稱。 在下一個帳單週期之前，此欄位會是空白的。 | *example.onmicrosoft.com* |
| 為 billingcycletype | 時間計費頻率。| **每月**  |
| 單位 | 資源**名稱**的單位。 | *GB*或*小時* |
| CustomerBillableAccount | Microsoft 計費平臺中的唯一帳戶識別碼。 | *1280018095* |
| UsageDate | 服務部署的日期。 | *2/1/2019 0:00* |
| MeteredRegion | 識別資料中心在區域內的位置（適用于並填入此值的服務）。 | *東亞*、*南部東亞*、*北歐*、西歐 *、**美國中北部*、*美國中南部* |
| MeteredService | 識別 [ **ServiceName** ] 資料行中未明確識別的個別 Azure 服務使用量。 例如，資料傳輸會回報為 Microsoft Azure-[ **ServiceName** ] 資料行中的*所有服務*。 | *AccessControl*， *CDN*，*計算*，*資料庫，資料**匯流排*，*儲存體* |
| MeteredServiceType | **MeteredService**欄位的子標題，可提供 Azure 服務使用量的額外說明。 | *外設* |
| Project | 客戶為其服務執行個體定義的名稱。 | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | 在指定一天布建和使用的 Azure 服務匯流排連接數目。 | *1.000000 個連線/30 天*（如果您在30天的一個月內有個別布建的連接）、 *25 個連接/30 天–使用： 1.000000* （如果您已布建25個服務匯流排連接，且在該日期期間使用了1個） |
