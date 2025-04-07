# Midterm

cd /var/www/html/
nano hack.php
cd /home/laurence/
cat hack.sh

cd /var/log/
sudo cat auth.log
sudo grep invalid auth.log | awk -F ' ' '{print $4}'
sudo grep invalid auth.log | awk -F ' ' '{print $3}' | sort | uniq
sudo grep invalid auth.log | awk -F ' ' '{print $4}' | sort | uniq
sudo grep invalid auth.log | awk -F ' ' '{print $4}' | sort | uniq
sudo grep 'Connection closed by invalid user' auth.log | awk -F ' ' '{print $12}' | grep -v USER | sort | uniq
sudo grep 'Connection closed by invalid user' auth.log | awk -F ' ' '{print $12}' | grep -v USER | sort | uniq > /home/jonasxie/invalid_ip.txt
sudo cat auth.log.1
sudo zcat auth.log.2.gz 

sudo zcat auth.log.2.gz | grep 'Disconnected from invalid user' | awk -F ' ' '{print $10}' | sort | uniq
sudo zcat auth.log.2.gz | grep 'Disconnected from invalid user' | awk -F ' ' '{print $11}' | sort | uniq
sudo zcat auth.log.2.gz | grep 'Disconnected from invalid user' | awk -F ' ' '{print $11}' | sort | uniq >> /home/jonasxie/invalid_ip.txt

sudo zcat auth.log.3.gz 
sudo zcat auth.log.3.gz | grep -i 'invalid'
sudo zcat auth.log.3.gz | grep 'Connection closed by invalid user' | awk -F ' ' '{print $11}' | sort | uniq 
sudo zcat auth.log.3.gz | grep 'Connection closed by invalid user' | awk -F ' ' '{print $12}' | sort | uniq 
sudo zcat auth.log.3.gz | grep 'Connection closed by invalid user' | awk -F ' ' '{print $12}' | sort | uniq >> /home/jonasxie/invalid_ip.txt

sudo grep 'session opened for user' auth.log
sudo grep 'session opened for user' auth.log | awk -F ' ' '{print $11}' | grep -v ';' | sort | uniq
sudo grep 'session opened for user' auth.log | awk -F ' ' '{print $11}' | grep -v ';' | sort | uniq >> /home/jonasxie/valid_ip.txt
sudo grep 'session opened for user' auth.log.1 | awk -F ' ' '{print $11}' | grep -v ';' | sort | uniq
sudo grep 'session opened for user' auth.log.1 | awk -F ' ' '{print $11}' | grep -v ';' | sort | uniq >> /home/jonasxie/valid_ip.txt

sudo zcat auth.log.2.gz | grep 'session opened for user' | awk -F ' ' '{print $11}' | grep -v ';' | sort | uniq
sudo zcat auth.log.2.gz | grep 'session opened for user' | awk -F ' ' '{print $11}' | grep -v ';' | sort | uniq >> /home/jonasxie/valid_ip.txt

cat /home/jonasxie/invalid_ip.txt | sort | uniq > /home/jonasxie/invalid_ip.txt
cat /home/jonasxie/valid_ip.txt | sort | uniq > /home/jonasxie/valid_ip.txt


sudo cat /etc/passwd | grep '/bin/bash' | awk -F ':' '{print $1} | grep -v 'jonasxie' | grep -v 'mlhess' | grep -v 'ubuntu'

cd /home
du -h --max-depth=1
cd raj
du -h --max-depth=1
cd mlhess
du -h --max-depth=1
ls

cd /home/laurence
ls
head -n 10 covid.csv
awk -F ',' '{print $2}' 'covid.csv' | sort | uniq | grep -v "state"
grep -v 'Hogwarts' covid.csv > /home/jonasxie/cleaned_covid.csv

cd /home/raj
cp food.csv /home/jonasxie/modified_food.csv
cd /home/jonasxie
sed s/unicorn/chicken/gI modified_food.csv > cleaned_food.csv



sudo cat /etc/passwd | grep '/home' | grep -v 'nologin' | grep -v 'mlhess' | grep -v 'jonasxie' | grep -v 'ubuntu' | awk -F ':' '{print $6} > /home/jonasxie/clean_folders.txt

