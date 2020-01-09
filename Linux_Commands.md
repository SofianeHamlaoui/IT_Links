|    | Command                                                                                                            | B                                         |
|----|---------------------------------------------------------------------------------------------------------------|-------------------------------------------|
| 1  | Centos 6                                                                                                      |                                           |
| 2  | netstat -uanp                                                                                                | udp                                       |
| 3  | netstat -tanp                                                                                                | tcp                                       |
| 4  | chkconfig                                                                                                     |                                           |
| 5  | service                                                                                                       |                                           |
| 6  | service network restart                                                                                       |                                           |
| 7  | service xinetd start                                                                                          |                                           |
| 8  | chkconfig telnet on                                                                                           |                                           |
| 9  | chkconfig xinetd on                                                                                           |                                           |                                                                                |                                           |
| 11 | sudo netstat -tuplen                                                                                         |                                           |
| 12 | netstat -an | grep                                                                                          |                                           |
| 13 | sudo tcpdump -n host 172.25.55.222 and port 3001                                                          |                                           |
| 14 | service iptables stop                                                                                         |                                           |
| 15 | /etc/init.d/iptables stop                                                                                    |                                           |
| 16 | chkconfig iptables off                                                                                        |                                           |
| 18 | ls -a <directory>                                                                                            | list all files in a directory plus hidden |
| 19 | yum whatprovides "*/qt5"                                                                                     |                                           |
| 20 | Yum install qt-devel qt-doc qt-creator qt5                                                                 |                                           |
| 21 | su -c 'yum update'                                                                                           |                                           |
| 23 | df -H                                                                                                        | List disk usage                           |
| 25 | ls -aR                                                                                                       |                                           |
| 27 | Using VIM, what is the findreplace function for replacing the word 'hot' with 'cold' in an entire document? |                                           |
| 28 | :%s/hot/cold/g                                                                                                |                                           |
| 32 | # chown root:root $file && chmod 1000 $file && chattr +iu $file                                             |                                           |
| 35 | In macOS, what are the default numeric file permissions on a user home folder; /Users/username/?              |                                           |
| 36 | drwxr-xr-x or 755                                                                                           |                                           |
| 38 | dig                                                                                                           |                                           |
| 40 | free -g                                                                                                      |                                           |
| 41 | df -h / df -i                                                                                               |                                           |
| 42 | uptime                                                                                                        |                                           |
| 43 | ps -ef | grep brsadmin | wc -l                                                                            |                                           |
| 44 | iostat                                                                                                        |                                           |
| 46 | exit the vi Editor                                                                                            |                                           |
| 47 | :x - Exit, saving changes                                                                                    |                                           |
| 48 | :q - Exit as long as there have been no changes                                                              |                                           |
| 50 | :q! - Exit and ignore any changes                                                                           |                                           |
| 51 | Ctrl + Z - Suspend editor                                                                                   |                                           |
