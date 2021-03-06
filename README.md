# simpleX
## a simple file explorer using index to browse under terminal
![](https://github.com/b2ns/simpleX/blob/master/demo.gif)
### install
just copy the shell script to ~/bin/ or anywhere else that has been added to $PATH  
type simplex to launch it.
### shortcut
```
use index(.e.g 1,2,3,4) to select a item:
'..' or 'u'                  go upper directory
'-' or 'b'                   go back
'r'                          refresh screen
'.'                          repeate last action
'.number'   .1 .2 .3         repeate a certain action
'~' or 'home'                go home
'/' or 'root'                go root
'm' or 'mark'                mark current directory
'g' or 'go'                  goto the marked directory
'b' or 'bookmark'            add current directory to bookmark
'bb'                         show all bookmarks
'rmb'    rmb 1               remove bookmark
'a' or 'all'                 show hidden files
'll'                         show detail
'mkf'                        make empty files
         mkf name1 name2 ...
'mkd'                        make directories
         mkd name1 name2 ...
'mkl'                        make soft link
         mkl index1 index2 ... or mkl * 
'del'                        delete
         del index1 index2 ... or del * 
'co' or 'copy'               copy to clipboard
         co index1 index2 ... or copy * 
'cu' or 'cut'                cut to clipboard
         cu index1 index2 ... or cut * 
'p' or 'paste'               paste
'rn'                         rename
         rn index1 name1 index2 name2 ...
'se' or 'fi'                 search
         se pattern
'pack'                       compress
         pack name index1 index2 ... or pack name * 
'unpack'                     decompress
         unpack index1 index2 ... or unpack * 
'q' or 'quit' or 'exit'      exit simpleX
```
### help
* the initial path will be the current path,you can start with other path by doing :  
  simplex path
* you can custom your own **alias** in simplex.alias
* default App is used to open a file
* after inputting 'a' or 'll' to show hidden file and detail,you can input it again to hide
* you can list files match certain pattern by using 'se',and deal with them all by using '*' afterwards such as del *, copy *,pack name *
* space and blank is not allowed while you name a file
* all common commands under terminal are supported,you can use them as long as you like;Besides,while dealing with files,you can use index to represent a certen file,for example: 
```
if there is a file named 'main.js' and the index of it is 23,you can do anything like :  
  vim main.js or vim 23  
  ls -l main.js or ls -l 23  
  cp main.js hello.js or cp 23 hello.js  
  rm -rf 23  
  tar -zcvf main.tar.gz 23  
below can be done with a 'n' before number because simpleX can't tell index from normal numbers:  
  chmod n640 23  
  echo {"name": "simpleX","array": [n1,n2,n3]} > 23  
  cat 23 | grep -E '[n0-n9]+'  
```
