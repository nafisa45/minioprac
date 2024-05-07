# minioprac terminal commands
hp@hp-HP-ProBook-440-G8-Notebook-PC:~$ cd ~/Desktop/python/minioConnect
hp@hp-HP-ProBook-440-G8-Notebook-PC:~/Desktop/python/minioConnect$ source venv/bin/activate
(venv) hp@hp-HP-ProBook-440-G8-Notebook-PC:~/Desktop/python/minioConnect$ pip install minio
Requirement already satisfied: minio in ./venv/lib/python3.10/site-packages (7.2.7)
Requirement already satisfied: urllib3 in ./venv/lib/python3.10/site-packages (from minio) (2.2.1)
Requirement already satisfied: argon2-cffi in ./venv/lib/python3.10/site-packages (from minio) (23.1.0)
Requirement already satisfied: certifi in ./venv/lib/python3.10/site-packages (from minio) (2024.2.2)
Requirement already satisfied: pycryptodome in ./venv/lib/python3.10/site-packages (from minio) (3.20.0)
Requirement already satisfied: typing-extensions in ./venv/lib/python3.10/site-packages (from minio) (4.11.0)
Requirement already satisfied: argon2-cffi-bindings in ./venv/lib/python3.10/site-packages (from argon2-cffi->minio) (21.2.0)
Requirement already satisfied: cffi>=1.0.1 in ./venv/lib/python3.10/site-packages (from argon2-cffi-bindings->argon2-cffi->minio) (1.16.0)
Requirement already satisfied: pycparser in ./venv/lib/python3.10/site-packages (from cffi>=1.0.1->argon2-cffi-bindings->argon2-cffi->minio) ((venv) hp@hp-HP-ProBook-440-G8-Notebook-PC:~/Desktop/python/minioConnect$ python3 minioConnect.py
Bucket 'testbucket' created successfully.
'flower.jpeg' is uploaded successfully to bucket 'testbucket'.
(venv) hp@hp-HP-ProBook-440-G8-Notebook-PC:~/Desktop/python/minioConnect$ python3 minioConnect.py
Bucket 'testbucket' already exists.
'flower.jpeg' is uploaded successfully to bucket 'testbucket'.
Traceback (most recent call last):
  File "/home/hp/Desktop/python/minioConnect/minioConnect.py", line 36, in <module>
    objects = client.list_objects("testbucket")
NameError: name 'client' is not defined
(venv) hp@hp-HP-ProBook-440-G8-Notebook-PC:~/Desktop/python/minioConnect$ cd testbucket
bash: cd: testbucket: No such file or directory
(venv) hp@hp-HP-ProBook-440-G8-Notebook-PC:~/Desktop/python/minioConnect$ ls
flower.jpeg  minioConnect.py  requirements.txt  venv
(venv) hp@hp-HP-ProBook-440-G8-Notebook-PC:~/Desktop/python/minioConnect$ cd ~/mdata
(venv) hp@hp-HP-ProBook-440-G8-Notebook-PC:~/mdata$ ll
total 16
drwxrwxrwx  4 hp hp 4096 May  8 01:28 ./
drwxr-x--- 55 hp hp 4096 May  8 01:17 ../
drwxr-xr-x  7 hp hp 4096 May  8 01:36 .minio.sys/
drwxr-xr-x  3 hp hp 4096 May  8 01:28 testbucket/
(venv) hp@hp-HP-ProBook-440-G8-Notebook-PC:~/mdata$ cd ~/testbucket
bash: cd: /home/hp/testbucket: No such file or directory
(venv) hp@hp-HP-ProBook-440-G8-Notebook-PC:~/mdata$ cd testbucket
(venv) hp@hp-HP-ProBook-440-G8-Notebook-PC:~/mdata/testbucket$ ll
total 12
drwxr-xr-x 3 hp hp 4096 May  8 01:28 ./
drwxrwxrwx 4 hp hp 4096 May  8 01:28 ../
drwxr-xr-x 3 hp hp 4096 May  8 01:30 flower.jpeg/
(venv) hp@hp-HP-ProBook-440-G8-Notebook-PC:~/mdata/testbucket$ 

