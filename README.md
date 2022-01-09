# community-nvt-feed-current

打版本时间 2022-01-09

## 打包成 tar.gz 格式，带压缩目录
```shell
tar -zcvf plugins.tar.gz ./plugins
tar -zcvf scap-data.tar.gz ./scap-data
tar -zcvf cert-data.tar.gz ./cert-data



## 打包成 tar.gz 格式，不带压缩目录

tar -zcvf plugins.tar.gz -C /var/lib/openvas/plugins .
tar -zcvf scap-data.tar.gz -C /var/lib/openvas/scap-data .
tar -zcvf cert-data.tar.gz -C /var/lib/openvas/cert-data .

## 解压 tar.gz 格式
tar -zxvf plugins.tar.gz -C /var/lib/openvas/
tar -zxvf scap-data.tar.gz -C /var/lib/openvas/
tar -zxvf cert-data.tar.gz -C /var/lib/openvas/


## 打包成 tar.bz2 格式，带压缩目录
tar -jcvf community-nvt-feed-current.tar.bz2 -C /var/lib/openvas plugins 
tar -jcvf plugins.tar.bz2 -C /var/lib/openvas plugins
tar -jcvf scap-data.tar.bz2 -C /var/lib/openvas scap-data
tar -jcvf cert-data.tar.bz2 -C /var/lib/openvas cert-data


## 打包成 tar.bz2 格式，不带带压缩目录
tar -jcvf community-nvt-feed-current.tar.bz2  -C /var/lib/openvas/plugins .
tar -jcvf community-nvt-feed-current.tar.bz2  -C ./plugins .
tar -jcvf plugins.tar.bz2 -C ./plugins .
tar -jcvf scap-data.tar.bz2 -C ./scap-data .
tar -jcvf cert-data.tar.bz2 -C ./cert-data .



## 解压 tar.bz2 格式
tar -jxvf plugins.tar.bz2 -C /var/lib/openvas/
tar -jxvf scap-data.tar.bz2 -C /var/lib/openvas/
tar -jxvf cert-data.tar.bz2 -C /var/lib/openvas/

## 复制文件夹
sudo cp -r ./plugins/ /var/lib/openvas/
sudo cp -r ./scap-data/ /var/lib/openvas/
sudo cp -r ./cert-data/ /var/lib/openvas/

```



