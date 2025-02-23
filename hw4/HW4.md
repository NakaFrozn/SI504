# Homework 4

**FROM:** Jonas Zhonghan Xie  
**TO:** Raj  
**SUBJECT:** RE: Questions about Database

Hi Raj,

Thanks for reaching out! I am happy to help with your questions about the text files in the database.

**Part 1**

1. Our database servers are hosted on Michigan Academic Computing Center (MACC) which is a large 2 MW data center located in Ann Arbor. The data center is equipped with backup power supplies, very reliable cooling systems (AC cooling aisles for example) and high-speed network connections. With the uninterrupted power supply (UPS) and the backup generators, the data center can be still running even in case of power outages. So don't worry about it. Our data will be safe. And the cooling systems are also very reliable. There are many cooling aisles, and the temperature is kept at a pretty constant level. The center is also equipped with well-designed fire suppression systems. 

2. I used `mkdir` to create a folder called `week4` in the home directory.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223145933.png)

3. I used `wget` to download the `pokemon.txt` in the directory.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223150118.png)

4. I used `grep -i` to count the occurrences of `Grass` and passed it to `wc -l` to count the lines. There are 95 'Grass Pokemons' in the file.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223150228.png)

5. I used the same command to count the occurrences of `Fire` and passed it to `wc -l` to count the lines. There are 64 'Fire Pokemons' in the file.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223150358.png)

6. I used `grep '711||` to locate the 711th pokemon in the file. It is Yveltal, a dark flying pokemon.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223150452.png)

1. I used `tail -n 5` command to show the last 5 lines in the pokemon file. 
The last five pokemon are "Dianche", "DiancieMega Diancie", "HoopaHoopa Confined", "HoopaHoopa Unbound", and "Volcanion".
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223150833.png)

**Part 2**

1. You can use `cat /etc/passwd | sort` to show the users in alphabetical order.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223151118.png)

1. I used `curl -s` to fetch the file and then used `grep` to find the lines that contain the word "props" and passed it to `wc -l` to count the lines. There are 53 lines containing the word, case insensitive.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223151738.png)

1. I used the same command to download, find the words. And then I passed the output to 'props.txt" using `> props.txt` command. The file is created in the directory.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223151850.png)
 
1. I first used `curl` to download the file and then used `grep -vi` to find the lines without "meetings", then passed it to `grep -i` to find the lines with "host", then passed it to `sort` and finally saved it to the file.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223152031.png)
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223152201.png)

**Part 3**:

1. There is only one CPU on my server.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223152628.png)

2. I used `du` command to show the disk usage of the current directory. My home directory takes up 26M space in total. The subdirectories (`--max-depth=1`) are also shown in the output.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223153920.png)

3. I used `ip a` and `grep` to locate the IP address and filtered out `inet6`.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250223154154.png)

Please let me know if you have any further questions. I am happy to help.

Best,  
Jonas