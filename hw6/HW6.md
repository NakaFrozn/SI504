# Homework 6

Hi Jack,

Hope you are doing well. I am happy to help with your requests.

1. My public key is as follows: ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQC+SJcH7/xkv4XEd2MrjDnGsMpT9wswMgnAH8zKe4JnE/ssygArStOA5DEoqfgboXxWV/PA25Fsj6tSqDnPpLIW4xDEjyixJWBBYhvYvSMA8ML8cBmWJKJDTamFVzc42p7Zvel6bdCCNnbVKEBsLMnhUvPamp1mZNGXsJp28B71/ohfO0gbjcWNkyyNsTGfgv0VQZvpUEFGpR/07iT3YAScv5WqHF5jkHSbhJR7Nl9k04HgssfIOnNwy48DxZSn2IaVEhiKBq7YK9fBH6YeMTjskMlREmqqSP5dvTzWDu6Mi45V6g/bcvPmYPQDONnAB0SUTQoXQ0ySF+a5mppdS+702SVFUOIg4Po77IlSpv3QemuwsfzVlKHgCqm5qNRwGN1XWjZoJwNI1tbC7LWyebEmjyqmfsYQe2LNx8lla/RpCY3g7wut6wwxHG0W54Z0J6JK/6XrV2j+3uTaF+vI6qOP4bqMvpAUujJHKSRgLlsgLSZtI75N3GXn9jPFjiGCYCE= jonasxie@ip-172-31-78-96
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250306213208.png)
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250306213215.png)

2. I first do `sudo apt-get update` to update the source. Then I used `sudo apt-get install apache2` to install Apache server. To download the zip file, I used `sudo wget` to download it and save it in `/var/www/html/`
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250306213614.png)

To unzip the files to the `/var/www/html/` directory, I used `sudo unzip zip.zip -d .` to unzip the files to current directory but not the subdirectory.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250306214000.png)

If you visit my IP address `http://44.200.214.242/`, you will see the nice website
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250306214251.png)

3. We need to use `sudo cp -r . /root` to copy all the files in home directory to root directory. We need to use `-r` to copy the directory recursively. We need to use `sudo` to get the permission to copy the files to root directory.
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250306214754.png)
![Alt text](%E5%BE%AE%E4%BF%A1%E6%88%AA%E5%9B%BE_20250306214759.png)

Let me know if you have any additional questions!

Best,  
Jonas