# Ubuntu-16.04.3安裝教學

> 本安裝教學是Gitlab安裝之前置步驟，需創建一台虛擬機並且依照Gitlab Installation的硬體需求來配置虛擬機設定，本教學亦可當作安裝ubuntu server之參考。

## 硬體需求
* 可參考[Gitlab安裝硬體需求](https://docs.gitlab.com/ce/install/requirements.html#hardware-requirements)。

## 軟體需求
請先至[ubuntu官方網站](https://www.ubuntu-tw.org/modules/tinyd0/)取得ubuntu-16.04-server的.iso檔案。

## 安裝步驟

1.建立好虛擬機後透過光碟機讀取ubuntu-16.04.3-server.iso，開始安裝流程。

2.選擇語言，這邊我們選擇「English」，點Enter繼續下一步。

![](/assets/ubuntu-installation_1.png)

3.選擇「Install Ubuntu Server」點Enter繼續下一步。

![](/assets/ubuntu-installation_2.png)

4.這邊是選擇安裝過程中的語言，我們選擇預設「English」，點Enter繼續下一步。

![](/assets/ubuntu-installation_3.png)

5.接著選擇使用伺服器的位置，如筆者的位置在台灣(Taiwan)，就選擇「亞洲(Asia)->台灣(Taiwan)」。範例一樣用預設「United States」，點「Enter」繼續下一步。

![](/assets/ubuntu-installation_4.png)

6.再來要設定鍵盤排列方式，沒有特殊需求的話，選擇「No」使用手動設定，並選擇「English(US)」就好。

![](/assets/ubuntu-installation_5.png)

7.這邊選擇「English（US）」。

![](/assets/ubuntu-installation_6.png)

8.選擇「English（US）」。

![](/assets/ubuntu-installation_7.png)

9.等待他載入額外元件。

![](/assets/ubuntu-installation_8.png)

10.如果有多張網路卡(網路介面)的話，選擇可以連上網際網路的那張。

![](/assets/ubuntu-installation_32.png)

11.輸入此ubuntu系統之hostname，這邊使用預設的「ubuntu」。

![](/assets/ubuntu-installation_9.png)

12.輸入要建立的預設user名稱，這邊輸入「ubuntu」。

![](/assets/ubuntu-installation_10.png)

13.輸入剛剛的user的username，這邊輸入「ubuntu」。

![](/assets/ubuntu-installation_11.png)

14.輸入此user的密碼。

![](/assets/ubuntu-installation_12.png)

15.再次輸入此user的密碼。

![](/assets/ubuntu-installation_13.png)

16.詢問是否要將home directory加密，這邊選擇「No」。

![](/assets/ubuntu-installation_14.png)

17.等待安裝系統偵測網路時區。

![](/assets/ubuntu-installation_15.png)

18.這邊詢問我們的時區是否是「Asia/Taipei」，選擇「Yes」確認。

![](/assets/ubuntu-installation_16.png)

19.這邊選擇分割儲存區的方式，我們選擇中間的「Guided - use entire disk and set up LVM」，因為是Server，所以建議使用LVM(Logical Volume Manager)來管理硬碟空間，方便日後的擴充。

![](/assets/ubuntu-installation_17.png)

20.選擇要使用的磁區，因為範例是虛擬機所以僅有一個磁區可用。

![](/assets/ubuntu-installation_18.png)

21.這邊是與我們確認是否要確定將上述資訊寫入磁區，選擇「Yes」。

![](/assets/ubuntu-installation_19.png)

22.點選「Continue」。

![](/assets/ubuntu-installation_20.png)

23.點選「Yes」，以上述設定寫入磁區。

![](/assets/ubuntu-installation_21.png)

24.等待系統安裝。

![](/assets/ubuntu-installation_22.png)

25.設定代理伺服器(Proxy)。若不設定代理伺服器，直接留空即可。

![](/assets/ubuntu-installation_23.png)

26.繼續等待Ubuntu Server安裝程式完成設定。

![](/assets/ubuntu-installation_24.png)

27.為了維持系統的穩定，可以選擇第一個「No automatic updates」用apt來自行進行手動更新，或者第二個「Install security updates automatically」設定自動更新安全相關系統程式。

![](/assets/ubuntu-installation_25.png)

28.選擇要額外安裝的軟體，我們通常會使用SSH來管理此ubuntu server，因此安裝了「OpenSSH Server」。

![](/assets/ubuntu-installation_26.png)

29.等候安裝。

![](/assets/ubuntu-installation_27.png)

30.選擇是否要安裝GRUB開機管理器。建議安裝，不然就要自己處理開機問題。

![](/assets/ubuntu-installation_28.png)

31.到這裡完成安裝，即可重新開機！

![](/assets/ubuntu-installation_29.png)

32.開機成功就可以看到Ubuntu Server的登入畫面。

![](/assets/ubuntu-installation_30.png)

33.輸入username及密碼即可成功登入系統。

![](/assets/ubuntu-installation_31.png)