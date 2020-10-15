# _<u>System Commands</u>_ #
<details>
<summary>**bzip2** _() -_ a block sorting file compression utility
</summary>

- -c 	create
- -v verbose
- -t test
</details>

<details>
<summary>**date** _(date +%F\ %r) -_ show system date and time
</summary>

- -%F	 full date
- -%r 12hr clock time
- -%u day of the week
- -%T 24hr time
</details>

<details>
<summary>**debugfs** _(debugfs /dev/hda1) -_ ext2/3/4 file system debugger
</summary>

- -w opens fs in read/write mode
</details>

<details>
<summary>**df** _(debugfs /dev/hda1)-_ ext2/3/4 file system debugger
</summary>

- -h human readable
- -T show filesystem type
</details>

<details>
<summary>**du** _(du -sh ~/Documents) -_ show disk usage of the filesystem
</summary>

- --max-depth=1
- -s summary
- -h human readable
</details>

<details>
<summary>**dumpe2fs** _(dumpe2fs -h /dev/sda3) -_ show filesystem info
</summary>

- -h human readable
</details>

<details>
<summary>**env** _(env) -_ show all environmental variables
</summary>

- -u unset variable
</details>

<details>
<summary>**fdisk** _(fdisk) -_ edit disk partition table
</summary>

- -p show current partitions
- -n create new partition 
- -d delete partition 
- -t change partition type
- -l list partition types
- -w save and quit
- -q quit without saving
</details>

<details>
<summary>**free** _(free) -_ show mem usage
</summary>

- -m megabytes
- -t totals
- -g gigabytes
</details>

<details>
<summary>**gzip** _(gzip -c miltext.doc) -_ compress files
</summary>

- -c create
- -l list compression stats
</details>

<details>
<summary>**kill** _(kill -9 1375) -_ send a process signal by PID
</summary>

- -9 force kill
- -15 send shutdown signal
</details>

**killall** _(killall apache2) -_ kill a process by name and assoc

<details>
<summary>**mke2fs** _(mke2fs -L /dev/DriveName) -_ make a ext2/3/4 filesystem
</summary>

- -L volume label
</details>


<details>
<summary>**mkfs** _(mkfs -t ext3 /dev/sda3) -_ make a linux filesystem
</summary>

- -t type
</details>

**nice** _(nice -15 google-chrome) -_ start a command with a set priority

**nohup** _(nohup google-chrome) –_ no hangups (run in backround)

**nproc** _(nproc) –_ show the # of processor cores

<details>
<summary>**renice** _(renice -20 gnome-shell) -_ change the priority of a command
</summary>

- -n scheduling priority
- -p change priority on a PID
- -g change priority on a group
- -u change priority on all a users processes
</details>

**pgrep** _(pgrep yumex)_ – show the PID using the process name

**ps** __(ps aux | grep miro)_ – list running processes

**source** _(source .bashrc)_ – reload a config file

**shopt** __(shopt -s histappend) -_ shell options

**shutdown** __(shutdown -r now) –_ shutdown the system

<details>
<summary>**tar** _(tar -cvpf testfile.tar.gz) -_ create an archive of files
</summary>

- -c create
- -r append files to end of an archive
- -t list contents of an achive
- -u update newer copies to archive
- -f use archive file
- -j bzip2
- -p preserve permissions
- -v verbose
- -z gzip
</details>

**telinit** _(teinit 6) –_ change the current runlevel of the system

<details>
<summary>**top** _(top -d 2) -_ show running task and stats
</summary>

- -d delay
- -U user
</details>

<details>
<summary>**tune2fs** _(tune2fs -c 120 /dev/sda1) -_ customize file system options on ext2/3/4 partitions
</summary>

- -c # of mounts before a filesystem check
- -i adjust fsck by time intervals
- -j add a journal to filesystem
- -m set reserve blocks used by root
- -r set reserve blocks by block #
- -L set volume label
- -U set UUID
</details>

**type** _(type ls) –_ show what a command is really doing

<details>
<summary>**uname** _(uname -a) -_ show system info
</summary>

- -a all
</details>

**uptime** __(uptime) –_ shows uptime and # of users

**w** __(w) –_ shows uptime, username and terminal

**which** _(which ping) –_ show the full path of shell commands

**whereis** _(whereis transmission) –_ locate the binary, source and man page

# _<u>User/Grp Commands</u>_ #

<details>
<summary>**useradd** _(useradd cream -d /home/cream -G sudo) -_ adds new user
</summary>

- -a add 
- -G add group
- -d custom home directory
</details>

<details>
<summary>**userdel** _(userdel -r Tom) -_ deletes user
</summary>

- -r recursive; removes home folder
</details>

**passwd** __(passwd) -_ change a users pw

<details>
<summary>**usermod** _(usermod -l Cream cream) -_ ext2/3/4 file system debugger
</summary>

- -l change login name
- -G add user to groups
- -s specify a shell
</details>

<details>

<summary>**groupadd** _(groupadd PowerUsers) -_ adds user groups to the system
</summary>

- -r on RH based systems to give the new group ID# under 500
</details>

**newgrp** _(newgrp Admins) -_ changes the users active group so the files created belong to that group

<details>
<summary>**gpasswd** _(gpasswd Admins) -_ used alone to change pw of the group
</summary>

- -A make someone admin of the group
- -a add as admin
- -d remove
</details>

<details>
<summary>**quotacheck** _(quotacheck -avcgum) -_ scan a filesystem for disk usage
</summary>

- -a all
- -v verbose
- -c create the file (aquota.usr or aquota.grp)
- -m force check without umounting the partition
- -g groups
- -u user
</details>

<details>
<summary>**edquota** _(edquota -u cream) -_ edit users quota space
</summary>

- -t set grace period
</details>

<details>
<summary>**repquota** _(repquota -u cream) -_ runs report of disk quota usage
</summary>

- -s print to screen
</details>


# _<u>File/Dir Commands</u>_ #

<details>
<summary>**awk** _(awk -F ‘:’ ‘{print $2}’) -_ data parsing
</summary>

- -F field separator
</details>

<details>
<summary>**cat** _(cat /etc/passwd) -_ concatenate and print files

**chattr** _(chattr ) -_ change attributes

**chmod** _(chmod 755 test1.txt) -_ change user permissions for files/directories

**chown** _(chown -R Admins /home/user/folder) -_ change ownership

<details>
<summary>**cut** _(grep “driver” ff.dat | cut -d\, -f2,3) -_ remove sections from each line of files
</summary>

- -d use delimiter
- -c character
- -b byte
- -f field
</details>

<details>
<summary>**find** _(find /home/cream -name shellcommands*) -_ find a file in a directory
</summary>

- -name proper name
- -amin files accessed +/- # minutes ago
- -atime files accessed +/- # hours ago
- -mmin files modified in the last +/- minutes ago
- -size M/G files of a certain siz
- -perm permission
- -user search by user
</details>

<details>
<summary>**grep** _(grep CompTIA*) -_ regular expression
</summary>

- -E extended reg expression
- -F fixed reg expression
- -e use as pattern
- -f text from file
- -w only whole words
- -i ignore case
- -n port numbers numbers
- -B/A 3 show lines before/after
- -C 2 show lines around(context)
- -r recursive search
- -l listening ports    
- -v        
</details>

<details>
<summary>**head** _(head -n 15 programlist1) -_ output the 1st 10 lines of a file
</summary>

- -n number of lines
</details>

**join** _(join test1.txt test2.txt) –_ join 2 files by similar fields

<details>
<summary>**locate** _(locate shellcommands.pdf) -_ find files by filename
</summary>

- -i ignore case
</details>

<details>
<summary>**ln** _(ln -s ~/target ~/linked) -_ create a link to a file
</summary>

- s soft link
</details>

<details>
<summary>**ls** _(ls -al /home/cream) -_ list files in the current directory
</summary>

- -a hidden files
- -l file permissions
</details>

**lsof** _(lsof) –_ list open files

**mkdir** _(mkdir ISOfiles) –_ make directory

<details>
<summary>**nl** _(nl filename) -_ # of lines of a file to display
</summary>

- -v start with line #
</details>

**od** _(od test1.txt) –_ dump files in octal format

**paste** _(paste file1 file2) –_ merges like # lines of 2 files

**pwd** _(pwd) –_ print working directory

<details>
<summary>**sed** _(sed s/assistant/assistant to/ message.txt) -_ (s)tandard (ed)itor for substituting text
</summary>

- s/ substitute
- /d delete
- /ii case insensitive
- /g global replace
- /1-9 # of occurrence on line to change
- -e,; execute multiple options
1-9 s/ # of line to change
</details>

<details>
<summary>**sort** _(sort /etc/passwd) -_ sort output a-z
</summary>

- -r reverse
- -n sort numbers
- -h human readable numbers
- -u unique values only
- -t change field separator
- -k             
</details>

<details>
<summary>**tail** _(tail file3) -_ view last 10 lines of a file
</summary>

- -n # of lines to show
</details>

<details>
<summary>**debugfs** _(debugfs /dev/hda1) -_ ext2/3/4 file system debugger
</summary>

- w opens fs in read/write mode
</details>

**tee** _(tee ) –_ read from standard input and write to standard output

**tr** _(echo myfoot.txt | tr o x) -_ translate characters in a file

<details>
<summary>**uniq** _(cat file1.txt | uniq -l) -_ show unique lines in a file
</summary>

- -d print duplicate lines
- -i ignore case
- -u unique lines
- -c count # of instances
- -k field
</details>

<details>
<summary>**wc** _(wc test3.txt) -_ print line, word and byte count for a file
</summary>

- -l # of lines
- -w # of words
- -c # of characters
</details>

# _<u>Network Commands</u>_ #

<details>
<summary>**arp** _(arp -e 192.168.1.24) -_ resolves IP addresses to MAC addresses
</summary>

- -s set entries
- -e Linux style
</details>

**dig** _(dig) –_ finds dns server name info

**ftp** _(ftp ) -_ file transfer protocol

**ifconfig** __(ifconfig eth0 192.168.1.124) –_ set or display network interface info 

<details>
<summary>**netstat** _(netstat -ntlp gmail.com) -_ show connections, routing table, interfaces, stats
</summary>

- -n supress name resolution, show numbers
- -t TCP
- -u UDP
- -l only listeners
- -a dump all sockets
- -r see routing table
- -p program name and PID#
- -i interface stats
</details>

**nmap** _(nmap google.com) –_ net explore tool and port scanner

**nslookup** _(nslookup) –_ find dns server name and address

**ping** _(ping -c 4) –_ ICMP echo command

**route** _(route 192.168.1.1) –_ display or set routing table info 

<details>
<summary>**tcpdump** _(tcpdump -i wlan0) -_ dump packets on a network, packet trace
</summary>

- -c count
</details>

**telnet** _(telnet 192.168.1.125 80) –_ check for open ports, or tty if ssh isnt available

**traceroute** _(traceroute gmail.com) –_ view the path data is taking to a destination

**whois** _(whois mmajunkie.com) –_ finds IP/domain ownership information

**a2enmod** _(a2enmod security) -_ enable apache module

**a2dismod** _(a2dismod imagemap) -_ disable apache module


### _<u>Git</u>_ ##

**git remote add origin** _(git remote add origin http://url) –_ add repo location

**git init** _(git init) -_ initialize the .git folder

**git add** _(git add .bashrc) -_ add a file to a git repository

<details>
<summary>**git commit** _(git commit -m “inital commit”) -_ commit file to a repo for upload
</summary>

- -a all
- -m message
</details>

<details>
<summary>**git push** _(git push -u origin .zshrc) -_ upload file to the repository
</summary>

- -u upstream
</details>

**git remote rm origin** _(git remote rm origin) -_ remove repo connection

**git pull** _(git pull http://...) -_ fetches and merges from repo
<details>
<summary>**git branch** _(git branch bashrc) -_ create new branch
</summary>

- -d delete
</details>

**git checkout** _(git checkout bashrc) –_ change to a different branch

**git clone** _(git clone http://...) -_ copy files in a repository

**git remote set-url origin** _(git...http://)-_change the remote repository url

**git push** _(git push -f origin master)-_ force push upstream to repo

**git merge** _(git merge footer-feature) -_ Join two or more branch histories together


### _<u>SSH</u>_ ##

**ssh** _(ssh cream@74.68.224.54) –_ secure socket connection

<details>
<summary>**ssh-keygen** _(ssh-keygen -t rsa) -_ generate keys for ssh authentication
</summary>

- -t type (rsa1,dsa,ecdsa,rsa)
- -C comment
</details>

**ssh-id-copy** _(ssh-id-copy -i ~/.ssh/rsa user@hostip) -_ copy ssh key to remote server



