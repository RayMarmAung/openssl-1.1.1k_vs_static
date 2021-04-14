# openssl-1.1.1k_vs_static
 Static build of openssl-1.1.1k With Visual Studio
- go https://www.openssl.org/source and download openssl source code desire your preferred version.
- i choose openssl-1.1.1k.tar.gz file, it's latest source code
- after downloaded, extract it, ie D:\openssl-1.1.1k\sources\openssl-1.1.1k
- To extract this, you may need 7z (download from this - https://www.7-zip.org/download.html)

![image](https://user-images.githubusercontent.com/17219341/114691586-d78f7100-9d3d-11eb-90f0-298cd8112b69.png)

- Before making any steps, you may need StrawBerryPerl (https://strawberryperl.com/) and Netwide Assembler NASM (https://www.nasm.us/)
- Execute Developer Command Prompt for VS as Run as administrator

![image](https://user-images.githubusercontent.com/17219341/114691741-fdb51100-9d3d-11eb-9ca2-e55f56c3bb3b.png)

- Change Source Directory with 'cd D:\openssl-1.1.1k\sources\openssl-1.1.1k'
- Configure with this command 'perl Configure VC-WIN32 --prefix=d:\openssl\builds\openssl-1.1.k-VC-WIN32'
- if you need to make static build, insert no-shared prompt 'perl Configure VC-WIN32 --prefix=d:\openssl\builds\openssl-1.1.1k-VC-WIN32 no-shared'

![image](https://user-images.githubusercontent.com/17219341/114692121-55ec1300-9d3e-11eb-97ec-95e33e6d1668.png)

- After Configuration finished, type this command to build and install 'nmake & nmake install'

![image](https://user-images.githubusercontent.com/17219341/114692307-859b1b00-9d3e-11eb-8300-665db0fd6558.png)

- Final Libraries can be used, it may request crypt32 and ws2_32 libs on vs project
