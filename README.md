# OpenAI_Intelligent_Agent

## Brief introduction
ESP32-S3 Large Model AI Development Kit is designed for developing scenarios involving large model voice interaction. It integrates peripheral components such as microphones, speakers, and OLED screens, and supports the use of OpenAI's large models.

Of course, you can also choose not to set up the environment and just use it directly. You can skip steps 1, 2, 3, 4, 5, and 6.

### 1、Pin diagram
![table](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/table.png)

### 2、Schematic
see the attachment.

## Firmware compilation
### 1、Download the offline installation package
We recommend using the ESP-IDF v5.3 version of IDF.
The official repository address of: https://github.com/espressif/esp-idf  
GitHub repository cloning command: git clone -b v5.3 --recursive https://github.com/espressif/esp-idf.git  
You also can dowm load IDF By selecting the IDF through the use of the official ESP manual: https://docs.espressif.com/projects/esp-idf/en/latest/esp32s3/api-reference/peripherals/isp.html
![step1](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/step1.png)
![step2](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/step2.png)
![step3](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/step3.png)

### 2、Install the Python environment
In order to prevent any issues with the mismatch of the computer's Python environment, we will first install the compatible version of the Python environment (Python-3.13.2-amd64).
Enter the website address in the browser: https://www.python.org/downloads/release/python-3132/

![py_install_step1](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/py_install_step1.png)
![py_install_step2](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/py_install_step2.png)
![py_install_step3](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/py_install_step3.png)
![py_install_step4](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/py_install_step4.png)
![py_install_step5](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/py_install_step5.png)

### 3、Install the ESP-IDF environment
Please select to install ESP-IDF version 5.3.                                                               

![idf_install_step1](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step1.png)
![idf_install_step2](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step2.png)
![idf_install_step3](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step3.png)
![idf_install_step4](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step4.png)
![idf_install_step5](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step5.png)

Just select default settings.                                                                                

![idf_install_step6](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step6.png)

Patiently wait for the installation to be complish.                                                                  

![idf_install_step7](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step7.png)
![idf_install_step8](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step8.png)
![idf_install_step9](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step9.png)
![idf_install_step10](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step10.png)


### 4、Check if the installation was successful### 4、Check if the installation was successful
If ESP-IDF 5.3 is installed on the computer, PowerShell can directly open the terminal.                  

![powershell_step1](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/powershell_step1.png)
![powershell_step2](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/powershell_step2.png)
When you see "idf.py build", it means the installation is successful and you can proceed to the next steps.

### 5、Set environment variables in the command window
#### 5.1、Open ESP-IDF PowerShell

![powershell_step1](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/powershell_step1.png)

#### 5.2、Update and download ESP-IDF tool.
Enter the Esp-idf folder and update the ESP-IDF tools for the Windows environment.
powershell:
cd C:\Espressif\frameworks\esp-idf-v5.3 (Fill in your own ESP-IDF storage path according to the actual situation).
.\install.bat (Update and download ESP-IDF tool)
![install_step1](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/install_step1.png)
![install_step2](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/install_step2.png)

Update finish.

#### 5.3、Set up the ESP-IDF environment.
Then, directly set the environment in the original path.
powershell:
.\export.bat
![export_step1](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/export_step1.png)
![export_step2](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/export_step2.png)

Set up finish.

#### 5.4、Has the test environment been set up successfully
Go directly to example and randomly select a project to run.               
powershell:
cd C:\Espressif\frameworks\esp-idf-v5.3\examples\get-started\hello_world\ (Fill in your own ESP-IDF storage path according to the actual situation). 

![test_step1](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/test_step1.png)

powershell:                                                                                            idf.py build

![test_step2](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/test_step2.png)

After pasting the code, press Enter and the compilation will start. During the compilation process, please make sure to turn off all antivirus software, such as Symantec, ESET, McAfee, etc., as this will significantly speed up the compilation process. (Please wait patiently for a moment.).

![test_step3](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/test_step3.png)
![test_step4](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/test_step4.png)

PS C:\Espressif\frameworks\esp-idf-v5.4\examples\get-started\hello_world> (based on the actual path) The code output at the same time shows no errors, meaning the compilation is complete.

### 6、Set up our ESP project
Our project is also located in the warehouse, in the folder named esp-webrtc-solution-main.       

It is recommended to create a folder named "esp" in the same level directory as esp-idf-v5.3, and place our code inside the "esp" folder.      

#### 6.1、Configure environment variables
In the search box of Windows 10 or Windows 11 (usually located at the bottom left corner of the taskbar), enter "env".
In the search results, click on "Edit System Environment Variables" or a similar option, and this will directly open the environment variable settings window.

![env_step1](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/env_step1.jpg)

Set the installation path of esp-webrtc-solution-main as the value of WEBRTC_SOLUTION_MAIN_PATH.       
If there is no path for esp-idf or esp-idf tools, please make sure to configure the corresponding paths.

Please make sure to close PowerShell!!! The reopen PowerShell.
Please make sure to close PowerShell!!! The reopen PowerShell.
Please make sure to close PowerShell!!! The reopen PowerShell.

#### 6.2、Running the script command
powershell:                                                                                            cd C:\Espressif\frameworks\esp\esp-webrtc-solution-main\solution\openai_demo\ (Fill in your own ESP-IDF storage path according to the actual situation). 
idf.py set-target esp32s3  (Set the target chip to esp32s3).

Explain:
1.<target> the target chip (It can be done through idf.py --list-targets check).
2.Clean build catalogue (use idf.py fullclean).
3.Delete sdkconfig flle (use mv sdkconfig sdkconfig.old).
4.Reconfigure the project using the new target chip (use idf.py -DIDF_TARGET=esp32 reconfigure).

Attention:                            
The command "idf.py set-target esp32s3" will clear the build files and the already configured menuconfig interface. You need to reconfigure it (do not perform this operation repeatedly without a good reason).

![settarget_step1.png](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/settarget_step1.png)

If the target chip reports an error, it might be because PowerShell was not properly closed and reopened, or the configuration information was not synchronized. Please close it and redo the entire 6.2 steps.                                    
If it still doesn't work, please turn off the device, restart it and then perform step 6.2 again.

If the above-mentioned approach still results in an error:
1.Please check if there are any other versions of Python               
Please check if your Python version is lower than 3.11. If so, please delete it. Make sure to install a compatible version of the Python environment (version 3.11 or above). If you have installed Python compilation software such as PyCharm, please check and delete other Python versions first.
2.Please check environment configure

![env_step1](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/env_step1.jpg)

Is the path configured correctly? Have the paths for idf, web_solution_main, and idf_tool all been set?

![settarget_step2](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/settarget_step2.png)

The error message means that the specified "build" directory does not appear to be a valid CMake build directory. The system refuses to automatically delete the files within it, and you need to manually delete this directory to perform the "cleaning" operation.

powershell:                                                                                            cd C:\Espressif\frameworks\esp\esp-webrtc-solution-main\solution\openai_demo\ (Fill in your own ESP-IDF storage path according to the actual situation). 
Remove-Item -Recurse -Force .\build
idf.py set-target esp32s3

If there no error message below,the configuration is successful.

![settarget_step3](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/settarget_step3.png)

#### 6.3、Build the Project
We don't need to use the idf.py menuconfig here. We can simply use the sdkconfig file in the folder instead.

![build_step1](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/build_step1.png)

If there is no error message,the configuration is successful.
If there is any error,please recheck the environment variables.

### 7、Create your own OpenAI agent
Create your own OpenAI agent need to go to the OpenAI website and create an account.

### 8、Set the necessary parameters
This is basically the final step. All you need to do is configure the SSID and password of the connected router, as well as the token you are using, and then you can start having conversations with our intelligent agent.

Set greeting phrases

![param_setting_step1.png](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/param_setting_step1.png)

At the beginning, if the WiFi connection fails, the device will enter the AP mode. You can access the website http://192.168.8.1 to complete the network configuration and set the token. The next time, this configuration will be automatically used and become the default configuration.

![param_setting_step2.png](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/param_setting_step2.png)
![param_setting_step3.png](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/param_setting_step3.png)
![param_setting_step4.png](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/param_setting_step4.png)
![param_setting_step5.png](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/param_setting_step5.png)
![param_setting_step6.png](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/param_setting_step6.png)
![param_setting_step7.png](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/param_setting_step7.png)
![param_setting_step8.png](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/param_setting_step8.png)

Then wait for a few seconds, and you can start the conversation.


