---

copyright:
  years: 2015, 2015


---


{:tsSymptoms: .tsSymptoms}
{:tsCauses: .tsCauses}
{:tsResolve: .tsResolve}
{:new_window: target="_blank"}  
{:shortdesc: .shortdesc}


# 一般服務問題
{: #general}

*前次更新：2016 年 8 月 12 日*
{: .last-updated}

{{site.data.keyword.Bluemix}} 服務問題可能包括刪除服務實例時發生的閘道逾時錯誤。然而，在許多情況下，您可以依照下列一些簡單的步驟，從這些問題中回復。
{:shortdesc}

## 刪除服務實例時發生服務分配管理系統錯誤
{: #ts_service_broker}

嘗試刪除已自雲端控制器中刪除的服務實例時，您可能會收到錯誤訊息。
{:shortdesc}


嘗試刪除服務實例時，您看到此服務分配管理系統錯誤訊息：`Gateway timeout`。
{: tsSymptoms}


如果服務實例已自雲端控制器中刪除，則會發生此問題。
{: tsCauses}


若要解決此問題，請建立具有相同服務名稱的服務實例，然後將它連結至應用程式。之後，您就可以刪除服務實例以及使用該服務的應用程式。   
{: tsResolve}
