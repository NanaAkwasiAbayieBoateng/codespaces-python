# codespaces-python
- Youtube video :  https://www.youtube.com/watch?v=gzh329Yzv8E
- github :  https://github.com/NanaAkwasiAbayieBoateng/compile-python
python codespaces
- update python 
``` sudo apt-get update```
- install python and libraies
``` 
sudo apt-get install build-essential gdb lcov libbz2-dev libffi-dev libgdbm-dev liblzma-dev libncurses5-dev libreadline6-dev libsqlite3-dev libssl-dev lzma lzma-dev tk-dev uuid-dev zlib1g-dev

```


- unzip and install python downloaded fro python website


```

 tar zxvf Python-3.10.5.tgz 

 ```

 - delete tar python file 
 ```
 rm Python-3.10.5.tgz 

 ```

 - change directory to python folder

 ```
 cd Python-3.10.5.tgz/

 ```

 - configure optimizations
 ```
  ./configure --enable-optimizations

  ```
- staurate all 8 cores
  ```
  make -j 8
  ```

  - put everything in place
  ```
  make altinstall 
  ```

  ```
  sudo make altinstall
  ```

  - switch from system installed python to local installed python

  ```
  cd ..
  /usr/local/bin/python3.10
  
  - make python default 
  ```
vim ~/.bashrc 
```

and add line: 

```
source ~/.venv/bin/activate
  ```


  - create requirements for python project
  ``` touch requirements.txt

  ```
- The Makefile will allow to setup github actions for continuous integration.
- Go to Actions then set up a workflow yourself 

  ``` touch Makefile
  ```

- install libraries in requirements.txt, this prints pip install -r requirements.txt
```
make install
```
