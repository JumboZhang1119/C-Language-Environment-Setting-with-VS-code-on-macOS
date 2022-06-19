C-Language Environment Setting with VS code on macOS
====
How to build your first C-Language environment setting on macOS with VS Code.
<br>
<br>
## For macOS user:
To build your C-Language environment, we can roughly divide the steps into the following 5 steps:
<br>
* Download Xcode
* Download VS Code
* Other setting
* Begin your first code

### Download Xcode
1. Go to `App Store` and download `Xcode`.<br><br>
<img width="1280" alt="02" src="https://user-images.githubusercontent.com/107752584/174472235-35a85be3-ce5b-4097-acbd-7803b6ac2dfd.png"><br><br>
2. Open the `terminal` and enter the code to install tools:
```
xcode-select –install
```
### Dowload VS Code
3. Go to [VS Code official website](https://code.visualstudio.com/) and click `Download Mac Universal`, then it will download automatically. <br><br>
![03](https://user-images.githubusercontent.com/107752584/174472471-916db038-2ec9-45bc-ad60-c32dc628b7c8.png)<br><br>
4. Open `VS Code App`, and click `Extensions` at the left side. Search `C/C++`, `C++ Intellisense`, `Code Runner` and download separately.<br><br>
![25](https://user-images.githubusercontent.com/107752584/174472568-9081062e-b49c-45a9-9edf-ee115c1dc897.png)
![26](https://user-images.githubusercontent.com/107752584/174472571-c6f1c641-58df-4519-bc8e-cf7a27a59b97.png)
![28](https://user-images.githubusercontent.com/107752584/174472574-3080500b-dbdf-4f5c-b29c-e2ba7cdafbf0.png)

### Other setting
5. Go to [vscode template for Mac](https://github.com/angel-star/vscode_template_for_Mac) and click `Code` > `Download ZIP`.<br><br>
![04](https://user-images.githubusercontent.com/107752584/174472706-2dfb7dce-32b1-4d05-944f-3e809f8a3039.png)<br><br>
6. Extract files and open it, then press `command + shift + .` to find `.vscode` folder.<br><br>
<img width="953" alt="截圖 2022-06-19 下午4 40 37" src="https://user-images.githubusercontent.com/107752584/174472973-2963ca27-a67f-4804-bdf7-a2b7f030cccb.png"><br><br>
7. Go to wherever you prefer to put your code in (For me I create a folder `CorC++`), and move the `.vscode` file from `vscode_template_for_Mac-master` to `your folder`(For me is `CorC++`).<br><br>
![截圖 2022-06-19 下午4 47 39](https://user-images.githubusercontent.com/107752584/174473168-743a0de6-55a3-4bb0-97b4-24169fc9e0b7.png)<br><br>
8. Go to your folder and press `control + click`, then click `get information`.<br><br>
![截圖 2022-06-19 下午4 57 48](https://user-images.githubusercontent.com/107752584/174473479-d65c68ec-e059-4f86-b988-504dbceaeb74.png)<br><br>
9. Press `control + click` at the position, then click `copy as pathname` to clone your folder path.<br><br>
<img width="262" alt="截圖 2022-06-19 下午5 01 26" src="https://user-images.githubusercontent.com/107752584/174473677-0340ac96-0547-4bca-98cc-99c87082b76d.png"><br><br>
11. In `VS Code App` click `File` > `Open Folder` and choose `your folder` (For me, I choose my `CorC++` folder).<br><br>
![截圖 2022-06-19 下午4 54 06](https://user-images.githubusercontent.com/107752584/174473322-a3878559-30d8-4240-b334-fedbd1d0adf0.png)<br><br>
12. Choose `c_cpp_properties.json`, and add your copied path under `macFrameworkPath`:
```
"Your Folder Path"
```
For me:
```
"/Users/zhangbaifeng/Documents/Coding/C/CorC++/"
```
![截圖 2022-06-19 下午5 06 23](https://user-images.githubusercontent.com/107752584/174474117-0c6d8290-3e04-4bd7-843e-75899863b4e6.png)<br><br>
13. Then you can create your file `XXXX.c (or XXXX.cpp)` in `.vscode`<br><br>

### Begin your first code!
14. You can try "Hello world!" for your first code!
```
#include <stdio.h>
int main() {
    printf("Hello World!\n");
    return 0;
}
```
![截圖 2022-06-19 下午5 16 21](https://user-images.githubusercontent.com/107752584/174474087-9bfafc60-738e-4c01-8874-39d736fb9a11.png)<br><br>
15. Then click `File` > `Auto Save`, and press `command + shift + B` to compile the code.<br><br>
<img width="1135" alt="截圖 2022-06-19 下午5 20 25" src="https://user-images.githubusercontent.com/107752584/174474208-c9101134-688b-4043-afc7-dc9213a3c717.png"><br><br>
16. Click that window and press any key to close it.<br>
17. Then drag form the VS Code window bottom to open the `TERMINAL` again.<br>
18. Enter: `./"your file name".out` to run your code (For me: `./test.out`).<br><br>
<img width="462" alt="截圖 2022-06-19 下午5 31 31" src="https://user-images.githubusercontent.com/107752584/174474637-27c12676-6909-4e4a-b947-d8f6dca89f6c.png"><br><br>
19. Note: Your `XXXX.c (or XXXX.cpp)` need to under the folder you created.<br><br>
<img width="410" alt="截圖 2022-06-19 下午5 38 35" src="https://user-images.githubusercontent.com/107752584/174474867-4181dba7-25bd-4d14-b802-6177448a12eb.png"><br><br>
20. Or you can just press `control + option + N` to run your code.<br><br>
<img width="792" alt="截圖 2022-06-19 下午5 41 33" src="https://user-images.githubusercontent.com/107752584/174475045-0a338d45-2dea-4145-94c9-e3edd5b08f54.png"><br><br>
## That's all!
