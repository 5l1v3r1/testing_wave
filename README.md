### ����

�þ�û�и����������ˣ������һ������������һ�����ӣ��������Һܴ�����һ��"web��ȫ��������©��ɨ����"����ȫ����Χ������������ʮ���web©��ɨ�����У��ҵ�ɨ������γ���? ������...����Ҳ���Ƕ�ô���ڣ�����������һ�߼�����Ա��һ��ʵս��web©���ھ�ѡ�־��ú�ʵ�ã���ʵ�ڣ�����������ڵġ�

��Ȼ��web©��ɨ��������ô��Ҫ�����˽���ʲô��web©���ھ�˵���˾����޸�http/s����������ݡ�

![](https://raw.githubusercontent.com/guimaizi/cloud/test/img/20200307181557.png)

��ͼ���ܱ�׵��һ��http�������Ҳ�Ǻܱ�׼��һ��xss©������ô�ж�xss�ķ�ʽ�����޸�name������ֵ��Ȼ���ж�http����Ӧ���ݣ�������ж�xss��©�����ڣ�ͨ�����ǻ��ֹ���name����׷��payload:

```<img src=a onerror=alert(1)>```

�ж���Ӧ�������ж����ǲ��Ǵ���һ��xss©��,����׷��' ��and 1=1��or 1=1��and sleep(3)���ж��Ƿ����sqlע��ȣ���������ĺ���ֵ���ÿ�ζ�����������ˮ���ˣ���ʤ�䷳����Ҳ�Ƿ��� �����ǺڿͰ�����Ȼ��ʼ����ˮ�߹����ˣ��ⲻ��ѧ��,̫ɵ����,��ô���ʱ�������Ҫ�����ɨ�����ˡ�

Ч����Ƶ: 

<video src="https://github.com/guimaizi/cloud/raw/test/20200307-190212967.mp4"/>

����get\post ���� Content-Type: application/json �����ɲ⡣

˼·���ǰ�burp��http�����ץ��������Ϊtmp.json

��ʽ:

```{
{"headers": 
    {
        "Origin": "http://192.168.0.137",
         "Cookie": "PHPSESSID=fjkq8kiuutn3hkoj4uppsg30da",
         "Accept": "application/json,
         text/javascript,
         */*; q=0.01",
         "X-Requested-With": "XMLHttpRequest",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML,
         like Gecko) Chrome/81.0.4009.0 Safari/537.36",
         "Referer": "http://192.168.0.137/12345.php",
         "Connection": "close",
         "Accept-Encoding": "gzip,
         deflate",
         "Accept-Language": "en-US,
        en;q=0.9",
         "Content-Length": "85",
         "Content-Type": "application/json"
    },
     "method": 1,
     "url": "http://192.168.0.137:80/12345.php",
     "post": "
    {
        \"userName\":\"asdas\",
        \"passWord\":\"dsadsa\",
        \"type\":1,
        \"data\":
        {
            \"aaaa\":\"bbbb\",
            \"cccc\":11111
        }
    }
    "
}
```

Ȼ��ͨ���ű�����׷��payload�� ���в���©����

������ [mitmproxy](https://github.com/mitmproxy/mitmproxy)   ��ô���Ǹ����Ʊ�Դ����[xray](https://github.com/chaitin/xray) �ı���ɨ������������������һ��ǿ������棬�Ǿ��Ǹ�����ɨ������

������Դ��,����������,��û�����

github: https://github.com/guimaizi/testing_wave



��ô�õĹ��ߣ���û�д�ү����Ը������һ�뼦�ҳ� wechat֧��:

![](https://raw.githubusercontent.com/guimaizi/cloud/test/img/20200307192617.png)



����/����/������ǰ �������뼦�ҳ�....

��ϵ��ʽWeChat : 

![](https://raw.githubusercontent.com/guimaizi/cloud/test/img/20200307193002.jpg)



