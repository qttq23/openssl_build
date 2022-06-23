1. download source (https://www.openssl.org/source/old/) (version 3.0) and unzip.

2. install tools: Stawberry-perl, nasm. then add those to PATH.

3. open 'x64 native tool command prompt' and go to openssl source root.

4. run:
perl Configure VC-WIN64A --prefix="%cd%/../../openssl_win32_x64_release" --openssldir="%cd%/../../ssl_win32_x64_release"

5. run:
nmake

6. run: (no need because it always failed. have no idea ??)
nmake test

7. run: 
nmake install

after installed, c++ project can use it. it works.