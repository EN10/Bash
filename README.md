#Bash Examples#

Bash Shortcut
-
File eg: 

    cd /mnt/c/folder/subfolder
    
Run:     

    . eg
    
Folder Size: 
-
    du -h --max-depth=1
    
Shorten Path:   
-
    PROMPT_DIRTRIM=1
    
Extract .tar.gz:    
-
    tar -xvzf filename.tar.gz
    
Bash ~ on windows:
-
    %localappdata%\Lxss\rootfs
    
Append a file:  
-
    echo "test" >> test.txt
    
File Word Frequency
-
    cat file | tr ' ' '\n' | sort | uniq -c
tr ' '  // remove multiple spaces   
'\n'    // output word per line