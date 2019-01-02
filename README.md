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

Command at Interval: 
-

    echo "date >> time" > time.sh
    watch -n 10 bash time.sh

Folder Size: 
-
Human readable, Max depth = 1

    du -hd1 /

File Size:
-
Sorted size human

    ls -Ssh /

Shorten Path:   
-
    PROMPT_DIRTRIM=1

Compress with `p7zip-full`
-
    7z a -mx9 -v100m compressedfilename filetocompress

`-mx9` compression level "ultra"  
`-v100m`  spilt into 100MB volumes

Extract 7z 
-

    7z e filename.7z

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

Find Installed Package
-
    sudo apt list --installed | grep -i lx

Installed Package By Size
-
    dpkg-query -Wf '${Installed-Size}\t${Package}\n' | sort -n
    
Purge Removed Packages
-
    dpkg --list |grep "^rc" | cut -d " " -f 3 | xargs sudo dpkg --purge

Find File
-
    find / -name *filename*

Bash ~ on windows:
-
    %localappdata%\Lxss\home