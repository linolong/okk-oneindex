# okk-oneindex

Parse error: syntax error, unexpected ''redis'' (T_CONSTANT_ENCAPSED_STRING), expecting ']' in /www/wwwroot/cloud.loftymountain.org/view/admin/settings.php on line 57

找到57行内容，替换nexmoe相应内容，解决问题，final为修改后的版本

伪静态如下

 <div class="snippet" markdown="1">

```
if (!-f $request_filename){
        set $rule_0 1$rule_0;
}
if (!-d $request_filename){
        set $rule_0 2$rule_0;
}
if ($rule_0 = "21"){
        rewrite ^/(.*)$ /index.php?/$1 last;
}

```
