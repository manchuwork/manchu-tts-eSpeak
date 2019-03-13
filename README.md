# manchu-tts-eSpeak
基于eSpeak http://espeak.sourceforge.net/

编译满族语言tts发音，满语发音，测试项目，很不完善
基于win平台的代码，D:\Program Files (x86)\eSpeak，安装（win平台依赖少些，开始启动快些）

主要修改文件
espeak目录
dictsource\mnc_list
dictsource\mnc_rule

phsource\ph_manchu  元音发音等
其他
espeak-data\oices\mnc
phsource\phonemes 引入mnc
语音相关

修改：安装eSpeak后，如下路径D:\Program Files (x86)\eSpeak 其他盘也可以
checkout 代码：
git clone git@github.com:manchuwork/manchu-tts-eSpeak.git eSpeak
当然，直接替换上面提到的文件也可以
将路径D:\Program Files (x86)\eSpeak\command_line加入path



编译文件：
```espeak --compile=mnc```
朗读测试：
``espeak -vmnc``
Unknown phoneme table: 'mnc'
na
ne
ni



备注：训练好的文件，可以放到其他的环境，有支持web发音的相关方案，直接在线朗读
