mysql --default-character-set=utf8 -h host -P port -uuser -ppwd dbname -A -e "SELECT * FROM tablename " | sed 's/ \|\[\|\]\|\"//g' | sed 's/,/;/g' | sed 's/\t/,/g'  > data/test.csv
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwNzE2ODQwMTNdfQ==
-->