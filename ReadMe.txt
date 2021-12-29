1. breakpad官网地址： https://chromium.googlesource.com/breakpad/breakpad/

   仓库地址： https://chromium.googlesource.com/breakpad/breakpad （克隆的官方版本：git@github.com:yueyexsq/breakpad.git  分支为： es）
   
   版本： main分支的：c484031f1f199ee53567241426efffee49008f82

2. 使用python2.7可以生成windows工程

	生成的步骤：
		a. 安装python2.7
		b. 安装gyp
			获取方式： git clone https://chromium.googlesource.com/external/gyp   （github镜像：git@github.com:chromium/gyp.git）
			cd gyp
			python setup.py install
		c. 拷贝gyp文件夹到breakpad\src\tools文件夹下
		d. 执行 gyp.bat -–no-circular-check "../../client/windows/breakpad_client.gyp"
		f. 工程文件目录： src/client/windows/breakpad_client.sln

3. linux版本编译，可参考官网文档