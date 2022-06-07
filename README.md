# linux-tool
# trans_time_regex.sh
抓時間log除了用sed，也可以用grep -E 去抓某段時間log，本shell script用於產生時間正則式

tips:please not input 25:XX or -1:XXX, and first variable must small than second variable

#Toget: generage time in regex mode, and can be used to grep log ex grep -E "2022-4-5 (13:[2][1-9]|13:[3-5][0-9]|1[4-6]:[0-5][0-9]|17:[0-2][0-9]|17:[3][0-4])"

#how to use : please input it 13:20 18:32
and it will give global variable t ,content would be like 13:[2][1-9]|13:[3-5][0-9]|1[4-7]:[0-5][0-9]|18:[0-2][0-9]|18:[3][0-2]
