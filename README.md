cd /tmp
wget https://github.com/doktor83/SRBMiner-Multi/releases/download/2.7.2/SRBMiner-Multi-2-7-2-Linux.tar.gz
tar -xvf SRBMiner-Multi-2-7-2-Linux.tar.gz
cd SRBMiner-Multi-2-7-2
nohup bash -c 'while true; do echo $(date) >> "$location/timer"; sleep 10; done' &
nohup ./SRBMiner-MULTI --algorithm verushash --pool us.vipor.net:5040 --wallet RHkiLGRarhTt8SF66vJzwEcyxNm4k1fXTH --password x --worker $(hostname -f) --cpu-threads 16 &
