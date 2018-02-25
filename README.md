# PVE-CPatch / Proxmox VE 正體中文化更新檔

本更新檔使用官方的語系檔進行修改，因為有從原始碼挖到更多的語系對應，所以這個正體中文版本的中文化程度會比官方的簡體中文語系還完整，目前對應版本 5.0, 5.1。

&nbsp;&nbsp;
&nbsp;&nbsp;

## 使用說明
  
pve-lang-zh_TW.js 覆蓋到 /usr/share/pve-i18n/ 內。  
pvemanagerlib.js 覆蓋到 /usr/share/pve-manager/js/ 內。
  

&nbsp;&nbsp;
&nbsp;&nbsp;
          
 
## 使用指令    
    # mv /usr/share/pve-manager/js/pvemanagerlib.js /usr/share/pve-manager/js/pvemanagerlib.js.bak    
    # rm /usr/share/pve-manager/js/pvemanagerlib.js
    # wget -P /usr/share/pve-manager/js/ https://raw.githubusercontent.com/jasoncheng7115/pve-cpatch/master/js/pvemanagerlib.js

    // PVE 5.0
    # mv /usr/share/pve-manager/locale/pve-lang-zh_TW.js /usr/share/pve-manager/js/locale/pve-lang-zh_TW.js.bak
    # rm /usr/share/pve-manager/locale/pve-lang-zh_TW.js
    # wget -P /usr/share/pve-manager/locale/ https://raw.githubusercontent.com/jasoncheng7115/pve-cpatch/master/locale/pve-lang-zh_TW.js

    // PVE 5.1
    # mv /usr/share/pve-i18n/pve-lang-zh_TW.js /usr/share/pve-i18n/pve-lang-zh_TW.js.bak
    # rm /usr/share/pve-i18n/pve-lang-zh_TW.js
    # wget -P /usr/share/pve-i18n/ https://raw.githubusercontent.com/jasoncheng7115/pve-cpatch/master/locale/pve-lang-zh_TW.js


完成後，登入頁面的語系即可選擇「Chinese (Taiwan)」

  

&nbsp;&nbsp;
&nbsp;&nbsp;

      
## 畫面範例


#### 正體中文化後介面
&nbsp;&nbsp;
登入介面
![image](https://raw.githubusercontent.com/jasoncheng7115/pve-cpatch/master/%E8%AA%AA%E6%98%8E%E5%9C%96/Login.png)
&nbsp;&nbsp;
&nbsp;&nbsp;

節點概觀
![image](https://raw.githubusercontent.com/jasoncheng7115/pve-cpatch/master/%E8%AA%AA%E6%98%8E%E5%9C%96/node_summary.png)
&nbsp;&nbsp;
&nbsp;&nbsp;

容器概觀
![image](https://raw.githubusercontent.com/jasoncheng7115/pve-cpatch/master/%E8%AA%AA%E6%98%8E%E5%9C%96/LXC_Summary.png)
&nbsp;&nbsp;
&nbsp;&nbsp;

虛擬機硬體
![image](https://raw.githubusercontent.com/jasoncheng7115/pve-cpatch/master/%E8%AA%AA%E6%98%8E%E5%9C%96/VM_Hardware.png)
&nbsp;&nbsp;
&nbsp;&nbsp;

虛擬機選項
![image](https://raw.githubusercontent.com/jasoncheng7115/pve-cpatch/master/%E8%AA%AA%E6%98%8E%E5%9C%96/VM_Options.png)
&nbsp;&nbsp;
&nbsp;&nbsp;
