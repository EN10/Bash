#Bash Examples#

Bash Shortcut
-
    
Run File eg:     

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
    
Append a file:  
-
    echo "test" >> test.txt
    
File Word Frequency
-
    cat file | tr ' ' '\n' | sort | uniq -c
tr ' '  // remove multiple spaces   
'\n'    // output word per line

Slim Git 
-

Light Git

    git clone --depth 1 https://github.com/EN10/chatbot.git
    
Files Only No Git

    svn export https://github.com/EN10/chatbot/trunk

Bash ~ on windows:
-
    %localappdata%\Lxss\rootfs