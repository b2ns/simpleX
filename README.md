# simpleX
## **a simple file explorer using index to browse under terminal**
![](https://github.com/b2ns/simpleX/blob/master/demo.gif)
## install
just copy the shell script to ~/bin/ or anywhere else that has been added to $PATH<br>
type simplex to launch it.
### shortcut
     use index(.e.g 1,2,3,4) to select a item
     'help'                       show help
     'shortcut'                   show shortcut
     '..' or 'u'                  go upper directory
     '-' or 'b'                   go back
     '.' or 'r'                   refresh screen
     '~' or 'home'                go home
     '/' or 'root'                go root
     'm' or 'mark'                mark a directory
     'g' or 'goto'                goto the marked directory
     'a' or 'all'                 show hidden files
     'll'                         show detail
     'mkfile'                     make empty files
              mkfile name1 name2 ...

     'mkdir'                      make directories
              mkdir name1 name2 ...

     'mklink'                     make soft link
              mklink index1 index2 ... or mklink * 

     'del'                        delete
              del index1 index2 ... or del * 

     'copy'                       copy to clipboard
              copy index1 index2 ... or copy * 

     'cut'                        cut to clipboard
              cut index1 index2 ... or cut * 

     'p' or 'paste'               paste
     'rn'                         rename
              rn index1 name1 index2 name2 ...

     'se'                         search
              se patten

     'pack'                       compress
              pack name index1 index2 ... or pack name * 

     'unpack'                     decompress
              unpack index1 index2 ... or unpack * 

     'q' or 'quit' or 'exit'      exit simpleX
    
### help
    1.the initial path will be the current path,you can start with other path by doing :
             simplex path
    2.you must use index(e.g. 2,45,998,142857) instead of file's name to select a file
    3.default App is used to open a file
    4.after inputting 'a' or 'll' to show hidden file and detail,you can input it again to hide
    5.space and blank is not allowed while you name a file
    6.you can list files match certain patter by using 'se',and deal with them all by using '*' afterwards such as del *, copy *,pack name *
    7.only support *.tar.gz,*.tar.bz2,*.tar.xz and *.zip
    8.all common commands under terminal are supported,you can use them as long as you like;Besides,while dealing with files,you can use a index starting with letter 'n'(e.g. n1,n23,n456) to represent a certen file,for example: 
        if there is a file named 'main.js' and the index of it is 23,you can do anything like :
                  vim main.js or vim n23
                  ls -l main.js or ls -l n23
                  cp main.js hello.js or cp n23 hello.js
                  rm -rf n23
                  chmod 640 n23
                  echo {"name": "simpleX","array": [1,2,3]} > n23
                  cat n23 | grep -E '[0-9]+'
                  tar -zcvf main.tar.gz n23
