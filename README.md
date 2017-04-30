# simpleX
**a simple file explorer using index to browse under terminal**
## help
     use index(number) to select a item
    'help'                       show help  
    'note'                       show note
    '..' or 'u' or 'up'          go upper directory
    '.' or 'r' or 'refresh'      refresh screen
    '~' or 'home'                go home
    '/' or 'root'                go root
    'm' or 'mark'                mark a directory
    'b' or 'back'                go back to a marked directory
    'a' or 'all'                 show hidden files
    'll'                         show detail  
    'mkfile'                     make empty files
             mkfile name1 name2 ...  
    'mkdir'                      make directories
             mkdir name1 name2 ...
    'mklink'                     make soft link
             mklink index1 name1 index2 name2 ...
    'rm' or 'del'                delete
             rm index1 index2 ... or rm * 
    'cp' or 'copy'               copy to clipboard
             cp index1 index2 ... or cp * 
    'cut'                        cut to clipboard
             cut index1 index2 ... or cut * 
    'p' or 'paste'               paste
    'rn' or 'rename'             rename
             rn index1 name1 index2 name2 ...
    'find'                       find
             find patten
    'tar'                        compress
             tar name index1 index2 ... or tar name * 
    'untar'                      decompress
             untar index1 index2 ... or untar * 
    'q' or 'quit' or 'exit'      exit simpleX
    
## note
    1.the initial path is home,you can start with other path by doing :
             `simplex path`
    2.you must use index instead of file's name to select a file
    3.after inputting 'a' or 'll' to show hidden file and detail,you can input it again to hide
    4.using 'b' or 'back' allows you to switch between current directory and a marked directory,just input it once again
    5.space and blank is not allowed while you name a file   
    6.you can list files match certain patter by using 'find',and deal with them all by using '*' afterwards such as rm *, cp *,tar name *
    7.only support *.tar.gz,*.tar.bz2,*.tar.xz and *.zip
    8.default App is used to open a file,you are allowed to choose another App to open it by doing :
             `AppName index`
    9.some simple command without options are supported,but can only take one parameter
    
