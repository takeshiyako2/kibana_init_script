# kibana_init_script

This is Kibana4 init script for CentOS.


# How to set up

Install Kibana4
```
cd /usr/local/src
wget https://download.elastic.co/kibana/kibana/kibana-4.1.1-linux-x64.tar.gz
tar xzf kibana-4.1.1-linux-x64.tar.gz
mv kibana-4.1.1-linux-x64 ../kibana
```

Clone init script
```
git clone git@github.com:takeshiyako2/kibana_init_script.git
cp kibana_init_script/kibana /etc/init.d/kibana
```

Start Kibana
```
chmod +x /etc/init.d/kibana
/etc/init.d/kibana start
```

Add kibana to chkconfig
```
chkconfig --add kibana
```

Check URL
```
curl http://192.168.33.10:5601/
```


# Origin

http://qiita.com/nagomu1985/items/82e699dde4f99b2ce417


