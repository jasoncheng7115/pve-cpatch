# PVE-CPatch / Proxmox VE 繁體中文化更新檔

本更新檔使用官方的語系檔進行修改，以台灣資訊用語為主，目前對應版本 5.0、5.1、5.2。

&nbsp;&nbsp;
&nbsp;&nbsp;

## 使用說明
5.0

  pve-lang-zh_TW.js 覆蓋到 /usr/share/pve-manager/locale/ 內。
  
  修改 /usr/share/pve-manager/js/pvemanagerlib.js 檔，加入繁體中文至 language_map 中。
  
5.1

  pve-lang-zh_TW_5.1.js 覆蓋到 /usr/share/pve-i18n/pve-lang-zh_TW.js。 
  
  修改 /usr/share/javascript/proxmox-widget-toolkit/proxmoxlib.js 檔，加入繁體中文至 language_map 中。

5.2

  pve-lang-zh_TW_5.2.js 覆蓋到 /usr/share/pve-i18n/pve-lang-zh_TW.js。 
  

&nbsp;&nbsp;
&nbsp;&nbsp;
          
 
## 使用指令    
    // PVE 5.0
    # mv /usr/share/pve-manager/locale/pve-lang-zh_TW.js /usr/share/pve-manager/js/locale/pve-lang-zh_TW.js.bak
    # rm /usr/share/pve-manager/locale/pve-lang-zh_TW.js
    # wget -P /usr/share/pve-manager/locale/ https://raw.githubusercontent.com/jasoncheng7115/pve-cpatch/master/locale/pve-lang-zh_TW.js

    // PVE 5.1
    # mv /usr/share/pve-i18n/pve-lang-zh_TW.js /usr/share/pve-i18n/pve-lang-zh_TW.js.bak
    # rm /usr/share/pve-i18n/pve-lang-zh_TW.js
    # wget -P /usr/share/pve-i18n/pve-lang-zh_TW.js https://raw.githubusercontent.com/jasoncheng7115/pve-cpatch/master/locale/pve-lang-zh_TW_5.1.js

    // PVE 5.2
    # mv /usr/share/pve-i18n/pve-lang-zh_TW.js /usr/share/pve-i18n/pve-lang-zh_TW.js.bak
    # rm /usr/share/pve-i18n/pve-lang-zh_TW.js
    # wget -P /usr/share/pve-i18n/pve-lang-zh_TW.js https://raw.githubusercontent.com/jasoncheng7115/pve-cpatch/master/locale/pve-lang-zh_TW_5.2.js

    // 修改 pvemanagerlib.js
    // 5.0 在 /usr/share/pve-manager/js/pvemanagerlib.js
    // 5.1 在 /usr/share/javascript/proxmox-widget-toolkit/proxmoxlib.js
    // 5.2 不需要修改這個檔案
    // 找到 language_map，加入正體中文
    ...
    language_map: {
        zh_CN: 'Chinese',
        zh_TW: 'Chinese(Taiwan)',
        ca: 'Catalan',
    ...
    

完成後，登入頁面的語系即可選擇「Chinese (Taiwan)」

  

&nbsp;&nbsp;
&nbsp;&nbsp;

      
## 畫面範例


#### 繁體中文化後介面
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
