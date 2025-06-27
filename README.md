# OpenAI_Intelligent_Agent

## Brief introduction
ESP32-S3 Large Model AI Development Kit is designed for developing scenarios involving large model voice interaction. It integrates peripheral components such as microphones, speakers, and OLED screens, and supports the use of OpenAI's large models.

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
![idf_install_step7](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step7.png)
![idf_install_step8](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step8.png)
![idf_install_step9](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step9.png)
![idf_install_step10](https://raw.githubusercontent.com/SabahEmperor/OpenAI_Intelligent_Agent/main/idf_install_step10.png)
Patiently wait for the installation to be compl

### 4、Check if the installation was successful


