# http-sniffer
对老版本的http嗅探器增加对http body的输出，添加过滤语句的使用
旧版本地址：https://github.com/caesar0301/http-sniffer
How to Use
Run scons in root folder to compile:

$ cd http-sniffer
$ scons
Get your live interface with ifconfig in terminal, e.g. en0, then

$ ./bin/http-sniffer -i en0
Or store output flows as json

$ ./bin/http-sniffer -i en0 -o output.json

Add the filter function

$ ./bin/http-sniffer  -i en0  -b  "host 10.10.10.10"  -o  output.json



