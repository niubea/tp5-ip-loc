# tp5-ip-loc
基于ThinkPHP5.1框架的ip地址查询库，可以针对ip地址进行查询，返回省份城市  
使用方法：  
1. 先在项目根目录composer require libo/tp5-ip-loc ；  
2. 在需要用到根据IP查地区的控制器里先use进来，代码如下：  
use libo\tp5_ip_loc\IPLoc;   
3. 在需要用到IP转地区的方法里使用以下代码：   
        $aa = new IPLoc();  
        $ipcity=$aa::find("113.111.183.221");  
        echo '<pre>'.print_r($ipcity).'</pre>';

