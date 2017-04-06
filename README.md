# Bash Examples

Create file1
-
    touch file1

Append a file1:  
-
    echo "text" >> file1.txt

Bash Shortcut
-
Run file1:     

    . file1

Folder Size: 
-
    du -h --max-depth=1
    
Shorten Path:   
-
    PROMPT_DIRTRIM=1
    
Extract .tar.gz:    
-
    tar -xvzf filename.tar.gz
    
Slim Git 
-

Light Git

    git clone --depth 1 https://github.com/EN10/chatbot.git
    
Files Only No Git

    svn export https://github.com/EN10/chatbot/trunk

Only Download Specific Folder   
Replace `tree/master` with `trunk`

    svn export https://github.com/GoogleCloudPlatform/python-docs-samples/trunk/appengine/standard/ndb/overview

File Word Frequency
-
    cat file | tr ' ' '\n' | sort | uniq -c
tr ' '  // remove multiple spaces   
'\n'    // output word per line

Bash ~ on windows:
-
    %localappdata%\Lxss\home