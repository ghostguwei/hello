Welcome to Git (version 1.9.4-preview20140929)


Run 'git help git' to display the help index.
Run 'git help <command>' to display help for specific commands.

Administrator@PC2014071419NAG /E/gitLocal (master)
$ ssh-keygen -t rsa -C "ghostguwei@126.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Documents and Settings/Administrator/.ss
h/id_rsa):
Created directory '/c/Documents and Settings/Administrator/.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Documents and Settings/Administrator/.s
sh/id_rsa.
Your public key has been saved in /c/Documents and Settings/Administrator/.ssh/i
d_rsa.pub.
The key fingerprint is:
1a:f5:34:4d:2f:e0:ba:18:ca:76:20:c2:0b:10:7b:78 ghostguwei@126.com
The key's randomart image is:
+--[ RSA 2048]----+
|.         . .    |
| +       . + .   |
|+ E     . + o .  |
|oo     . + . .   |
|o.. . o S .      |
|...o o = .       |
| .  + + .        |
|   . .           |
|                 |
+-----------------+

Administrator@PC2014071419NAG /E/gitLocal (master)
$ ssh -T git@github.com
The authenticity of host 'github.com (192.30.252.128)' can't be established.
RSA key fingerprint is 16:27:ac:a5:76:28:2d:36:63:1b:56:4d:eb:df:a6:48.
Are you sure you want to continue connecting (yes/no)? yes
Warning: Permanently added 'github.com,192.30.252.128' (RSA) to the list of know
n hosts.
Hi ghostguwei! You've successfully authenticated, but GitHub does not provide sh
ell access.

Administrator@PC2014071419NAG /E/gitLocal (master)
$ git config --global user.name "guwei"

Administrator@PC2014071419NAG /E/gitLocal (master)
$ git config --global user.email "ghostguwei@126.com"

Administrator@PC2014071419NAG /E/gitLocal (master)
$ git remote add origin git@github.com:ghostguwei/hello

Administrator@PC2014071419NAG /E/gitLocal (master)
$ git add readMe.txt

Administrator@PC2014071419NAG /E/gitLocal (master)
$ git commit -m "first commit"
[master (root-commit) 0687188] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 readMe.txt

Administrator@PC2014071419NAG /E/gitLocal (master)
$ git push origin master
Warning: Permanently added the RSA host key for IP address '192.30.252.131' to t
he list of known hosts.
To git@github.com:ghostguwei/hello
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'git@github.com:ghostguwei/hello'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Administrator@PC2014071419NAG /E/gitLocal (master)
$ git pull origin master
Warning: Permanently added the RSA host key for IP address '192.30.252.130' to t
he list of known hosts.
warning: no common commits
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0)
Unpacking objects: 100% (3/3), done.
From github.com:ghostguwei/hello
 * branch            master     -> FETCH_HEAD
 * [new branch]      master     -> origin/master
Merge made by the 'recursive' strategy.
 README.md | 4 ++++
 1 file changed, 4 insertions(+)
 create mode 100644 README.md

Administrator@PC2014071419NAG /E/gitLocal (master)
$ git push origin master
Warning: Permanently added the RSA host key for IP address '192.30.252.129' to t
he list of known hosts.
Counting objects: 6, done.
Delta compression using up to 2 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (5/5), 496 bytes | 0 bytes/s, done.
Total 5 (delta 0), reused 0 (delta 0)
To git@github.com:ghostguwei/hello
   dfde00e..47e7933  master -> master

Administrator@PC2014071419NAG /E/gitLocal (master)
$