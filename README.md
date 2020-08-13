# Web Scanner Sample
The sample shows how to scan documents to web browsers via IP address with Dynamic Web TWAIN.

## How Dynamic Web TWAIN Works for Remote Scanner Access

![Dynamic Web TWAIN remote scan](https://www.dynamsoft.com/codepool/wp-content/uploads/2020/08/dynamic-web-twain-remote-scanner-workflow.png)

## How to Configure Dynamsoft Service 
1. Install [Dynamic Web TWAIN SDK](https://www.dynamsoft.com/Downloads/WebTWAIN_Download.aspx) and run `Dynamsoft Service` on `Windows`, `Linux`, `macOS` or `Raspberry Pi OS`.
2. Add your machine IP address to `DSConfiguration.ini`:

    ```
    Server=<MACHINE IP ADDRESS>
    ```
    
    - Windows: C:\Windows\SysWOW64\Dynamsoft\DynamsoftServicex64_16\DSConfiguration.ini
    
      ![Windows remote scan configuration](https://www.dynamsoft.com/codepool/wp-content/uploads/2020/08/windows-remote-scan-configuration.png)
      
    - Linux, macOS and Raspberry Pi OS: /opt/dynamsoft/DynamsoftService/DSConfiguration.ini
      
      ![Linux remote scan configuration](https://www.dynamsoft.com/codepool/wp-content/uploads/2020/08/linux-remote-scan-configuration.png)
3. Copy `Dynamic Web TWAIN SDK <version number>/Resources` folder to the project directory.

## How to Make the Sample Work
1. Update the IP address according to your configuration:

    ```html
    <option>192.168.8.84</option>
    <option>192.168.8.85</option>
    ```
   
2. Get a valid [license key](https://www.dynamsoft.com/CustomerPortal/Portal/Triallicense.aspx) and update the following code:
 
    ```js
    Dynamsoft.WebTwainEnv.ProductKey = 'LICENSE-KEY';
    ```
    
3. Deploy the `index.htm` file to your web server.
4. Visit the web app in your desktop or mobile web browsers. 

    ![capture documents via mobile scanner](https://www.dynamsoft.com/codepool/wp-content/uploads/2020/08/remote-scanner-document.jpg)
    
    ![scanner IP address](https://www.dynamsoft.com/codepool/wp-content/uploads/2020/08/web-remote-scanner-source.jpg)
    
