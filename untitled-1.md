# Logic App

{% embed data="{\"url\":\"https://docs.microsoft.com/en-us/azure/logic-apps/quickstart-create-first-logic-app-workflow\",\"type\":\"link\",\"title\":\"Create your first automated workflow - Azure Logic Apps\",\"description\":\"This quickstart shows how to automate your first workflow with Azure Logic Apps for system integration and enterprise application integration \(EAI\) scenarios that integrate systems & cloud services\",\"icon\":{\"type\":\"icon\",\"url\":\"https://docs.microsoft.com/favicon.ico\",\"aspectRatio\":0},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://docs.microsoft.com/\_themes/docs.theme/master/en-us/\_themes/images/microsoft-header.png\",\"width\":128,\"height\":128,\"aspectRatio\":1}}" %}

## Logic app: Monitoring social media

Zacznijmy od założenia konta na Twitterze.

 Następnie stwórz nowy zasób - **Aplikację logiki **\(ang. _Logic app_\).

![](.gitbook/assets/image%20%288%29.png)

Stwórzmy pustą aplikację, w której będziemy monitorować tweety z hashtagiem **"\#MSPBuzz"**. W tym celu wybierz wyzwalacz **"Po wysłaniu nowego tweetu".**

![](.gitbook/assets/image%20%2812%29.png)

Wysyłamy maila o wykryciu nowego tweeta:



![](.gitbook/assets/image%20%287%29.png)

## Omówienie Cognitive Services

{% embed data="{\"url\":\"https://azure.microsoft.com/en-us/services/cognitive-services/\",\"type\":\"link\",\"title\":\"Cognitive Services \| Microsoft Azure\",\"description\":\"Add vision, speech, language and knowledge capabilities to your apps with artificial intelligence APIs from Cognitive Services. Explore our APIs today.\",\"icon\":{\"type\":\"icon\",\"url\":\"https://azurecomcdn.azureedge.net/cvt-a845dff1bcbf674c04a243c4798ba0e4eb81d06669d01df49ba5367ed02881d5/images/icon/apple-touch/180x180.png\",\"width\":180,\"height\":180,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://azurecomcdn.azureedge.net/cvt-4ba1ac63410bb2bbe9f1c2a7bedc57894bbe9754309d9d380deedcdf7850047e/images/shared/social/azure-icon-250x250.png\",\"width\":250,\"height\":250,\"aspectRatio\":1}}" %}

## Logic app: Analiza social media

Aby reagować szybciej na negatywny feedback chcielibyśmy wykryć go spośród pozytywnych informacji, które otrzymujemy.

Zacznijmy od utworzenia zasobu **Text Analysis API**

{% embed data="{\"url\":\"https://docs.microsoft.com/pl-pl/azure/cognitive-services/text-analytics/\",\"type\":\"link\",\"title\":\"Azure Cognitive Services, Text Analytics API Documentation - Tutorials, API Reference\",\"description\":\"Learn how to create and develop apps using Text Analytics API\",\"icon\":{\"type\":\"icon\",\"url\":\"https://docs.microsoft.com/favicon.ico\",\"aspectRatio\":0},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://docs.microsoft.com/\_themes/docs.theme/master/en-us/\_themes/images/microsoft-header.png\",\"width\":128,\"height\":128,\"aspectRatio\":1}}" %}

Następnie w naszej aplikacji logiki tłumaczymy tweeta na język angielski:



![](.gitbook/assets/image%20%2816%29.png)

I analizujemy go pod względem zawartości:



![](.gitbook/assets/image%20%281%29.png)

Zależnie od wyniku podejmujemy różne działania:



![](.gitbook/assets/image%20%2817%29.png)

