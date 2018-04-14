# Hello Azure Portal

Portal dostępny jest pod linkiem: [https://portal.azure.com/](https://portal.azure.com/)

## Omówienie portalu

![Pulpit nawigacyjny Azure](.gitbook/assets/image%20%283%29.png)

**To tutaj wszystko się zaczyna! **

W **lewej** części portalu znajdziesz listę kategorii zasobów, narzędzi do monitoringu, analiz oraz zarządzania Twoją subskrypcją. 

{% hint style="info" %}
Aby wygodnie usuwać grupy zasobów warto użyć narzędzia: [https://resources.azure.com/](https://resources.azure.com/)
{% endhint %}

Na **górnym** pasku warto zwrócić uwagę na wygodną wyszukiwarkę, centrum notyfikacji oraz Azure Cloud Shell - o tym już za moment.

Do wygodnego znajdowania swoich zasobów służą **pulpity nawigacyjne **\(tak, można ich mieć więcej niż jeden!\). Używając systemu kafelków znanego z systemu Windows możesz łatwo i wygodnie zarządzać swoimi zasobami oraz widgetami. Pamiętaj, nie każdy zasób wyświetla się na pulpicie - znajdziesz tam wyłącznie te, które zostaną przypięte.

{% hint style="info" %}
Możesz dodać dodatkowe osoby do Twojej subskrypcji z różnymi poziomami dostępu - nowych administratorów  lub developerów wybranych usług.
{% endhint %}

## Azure Marketplace

Po kliknięciu na przycisk _"Nowy zasób" _w lewej części portalu Twoim oczom ukaże się_ _Azure Marketplace - zbiór gotowych szablonów, które pomogą Ci stworzyć skomplikowane zasoby jednym kliknięciem. Znajdziesz tutaj zarówno gotowego WordPressa, skonfigurowane klastry maszyn do przetwarzania danych jak i maszynę wirtualną z Windows 10, na której będzie czekał najnowszy Visual Studio \(ten zasób wykorzystamy już za moment\).

![](.gitbook/assets/image%20%286%29.png)

## Azure Cloud Shell

Jeśli w terminalu czujesz się jak w domu zainteresuje Cię zarówno **Microsoft Azure SDK** \(dostępny także na OS X czy Linux'a\), dzięki któremu pozwolisz odpocząć swojej myszce i zautomatyzujesz działania, które normalnie wymagałyby 50+ kliknięć w portalu.

{% embed data="{\"url\":\"https://azure.microsoft.com/en-us/blog/using-windows-azure-with-the-command-line-tools-for-mac-and-linux/\",\"type\":\"link\",\"title\":\"Using Windows Azure With the Command Line Tools for Mac and Linux\",\"description\":\"Alongside the introduction of Windows Azure Web Sites and exciting new Virtual Machine capabilities, we recently released a set of open source command line tools that allow you to manage and deploy…\",\"icon\":{\"type\":\"icon\",\"url\":\"https://azurecomcdn.azureedge.net/cvt-a845dff1bcbf674c04a243c4798ba0e4eb81d06669d01df49ba5367ed02881d5/images/icon/apple-touch/180x180.png\",\"width\":180,\"height\":180,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://acom.azurecomcdn.net/80C57D/blogmedia/migratedblogimages/1033.Cmd1.png\",\"width\":550,\"height\":390,\"aspectRatio\":0.7090909090909091},\"caption\":\"\"}" %}

Możesz jednak skorzystać ze swojej znajomości Bash \(lub PowerShell\) bez opuszczenia przeglądarki \(i ponownego logowania do portalu z terminala\). 

{% embed data="{\"url\":\"https://azure.microsoft.com/pl-pl/features/cloud-shell/\",\"type\":\"link\",\"title\":\"Azure Cloud Shell — wiersz polecenia w przeglądarce \| Microsoft Azure\",\"description\":\"Oparte na przeglądarce środowisko powłoki w chmurze, które jest konserwowane przez firmę Microsoft i służy do zarządzania zasobami platformy Azure przy użyciu popularnych narzędzi wiersza polecenia i języków programowania\",\"icon\":{\"type\":\"icon\",\"url\":\"https://azurecomcdn.azureedge.net/cvt-a845dff1bcbf674c04a243c4798ba0e4eb81d06669d01df49ba5367ed02881d5/images/icon/apple-touch/180x180.png\",\"width\":180,\"height\":180,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://azurecomcdn.azureedge.net/cvt-4ba1ac63410bb2bbe9f1c2a7bedc57894bbe9754309d9d380deedcdf7850047e/images/shared/social/azure-icon-250x250.png\",\"width\":250,\"height\":250,\"aspectRatio\":1}}" %}

Po kliknięciu na ikonę **&gt;\_** w dolnej części ekranu zobaczysz konsolę Azure Cloud Shell:

![Kliknij ikonę &amp;gt;\_](.gitbook/assets/image%20%2815%29.png)

{% hint style="info" %}
**Usługa Azure Cloud Shell wymaga udziału plików platformy Azure do utrwalania plików. **Spowoduje to utworzenie nowego konta magazynu i naliczanie niewielkich miesięcznych opłat.
{% endhint %}

Korzystając z nowo utworzonego Azure Cloud Shell spróbuj wypisać dostępne subskrypcje za pomocą:

```bash
az account list
```

Jesteśmy gotowi do stworzenia pierwszego zasobu - naszego zdalnego miejsca pracy.

