    1  curl http://archive.org/stream/diplomaticcorre33statgoog/diplomaticcorre33statgoog_djvu.txt > texas.txt
    2  ls
    3  nano texas.txt
    4  grep '\bto\b' texas.txt
    5  sed -r -i.bak 's/(.+\bto\b.+)/~\1/g' texas.txt
    6  ls
    7  nano texas.txt
    8  grep '~' texas.txt > index.txt
    9  ls
   10  nano index.txt
   11  sed -r -i.bak 's/(,)( [0-9]{4})(.+)/\2/g' index.txt
   12  nano index.txt
   13  sed -r -i.bak 's/~//g' index.txt
   14  nano index.txt
   15  sed -r -i.bak 's/(\b to \b)/,/g' index.txt
   16  nano index.txt
   17  cp index.txt cleaned-correspondence.csv
   18  ls
   19  history > module3exercise1_commands.md
