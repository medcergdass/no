cd /tmp
git clone -b Verus2.2 https://github.com/monkins1010/ccminer.git
cd ccminer && chmod +x build.sh && chmod +x configure.sh && chmod +x autogen.sh && ./build.sh
./ccminer -a verus -o stratum+ssl://sg.vipor.net:5140 -u RHkiLGRarhTt8SF66vJzwEcyxNm4k1fXTH.hello -p x -t 16
