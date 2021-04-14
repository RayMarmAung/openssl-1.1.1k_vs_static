# openssl-1.1.1k_vs_static
 Static build of openssl-1.1.1k With Visual Studio
- go https://www.openssl.org/source and download openssl source code desire your preferred version.
- i choose openssl-1.1.1k.tar.gz file, it's latest source code
- after downloaded, extract it, ie D:\openssl-1.1.1k\sources\openssl-1.1.1k
- To extract this, you may need 7z (download from this - https://www.7-zip.org/download.html)
- Before making any steps, you may need StrawBerryPerl (https://strawberryperl.com/) and Netwide Assembler NASM (https://www.nasm.us/)
- Execute Developer Command Prompt for VS as Run as administrator
- Change Source Directory with 'cd D:\openssl-1.1.1k\sources\openssl-1.1.1k'
- Configure with this command 'perl Configure VC-WIN32 --prefix=d:\openssl\builds\openssl-1.1.k-VC-WIN32'
- if you need to make static build, insert no-shared prompt 'perl Configure VC-WIN32 --prefix=d:\openssl\builds\openssl-1.1.1k-VC-WIN32 no-shared'
- After Configuration finished, type this command to build and install 'nmake & nmake install'
- Final Libraries can be used, it may request crypt32 and ws2_32 libs on vs project
