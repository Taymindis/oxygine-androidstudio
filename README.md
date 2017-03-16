# oxygine-androidstudio
This is a sample program from oxygine-framework https://github.com/oxygine/oxygine-framework , and able to build and debug c++ with android studio

## Steps
### 1. clone the latest oxygine-framework from https://github.com/oxygine/oxygine-framework and download the latest SDL2 and rename it to SDL and put at the same peer directory with oxygine-framework
#### 1.1 then build your project by execute ${OXYGINE_FRAMEWORK}/examples/HelloWorld/proj.android/build-run.sh


### 2. Open android studio and click import project the select ${OXYGINE_FRAMEWORK}/examples/HelloWorld/proj.android/build.gradle



### 3. Go to Project Structure and setup the SDK and NDK path of this project.




### 4. Add ndk-build closure in ${OXYGINE_FRAMEWORK}/examples/HelloWorld/proj.android/build.gradle. Then try to build it by execute assembleDebug from android-studio UI






### 5. After build successfully, you will see the unstripped lib folder generated at ${OXYGINE_FRAMEWORK}/examples/HelloWorld/proj.android/obj/local/armeabi-v7a , Go to Run tab->edit configuration->Debugger tab and follow the screen below:-



#### add symbol directories differentiate by ABI. eg. 
${OXYGINE_FRAMEWORK}/examples/HelloWorld/proj.android/obj/local/armeabi-v7a
${OXYGINE_FRAMEWORK}/examples/HelloWorld/proj.android/obj/local/x86
..


### 6. you may now to deploy to your mobile by press debug to mobile/emulator and debug your cpp application

