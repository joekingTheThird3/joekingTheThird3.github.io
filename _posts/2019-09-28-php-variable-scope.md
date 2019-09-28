---
categories: [php,code,scope]
tags: [php,code,scope]
layout: post
title: "php variable scope"
date: 2019-09-28
salute: hello
myarray: ['item1','item2','item3']
myhash: {
'key1':'item1',
'key2':'item2',
'key3':'item3'
}
---
{% raw %}
<img src="https://github.com/joekingTheThird3/joekingTheThird3.github.io/blob/master/assets/28-09-2019-0375.png?raw=true">
<br>
output of previous code
<br>
<img src="https://raw.githubusercontent.com/joekingTheThird3/joekingTheThird3.github.io/master/assets/28-09-2019-0374.png?raw=true">
{% endraw %}


So, what happens?
$foo is global. In the function the variable $foo is accessed by the 'global' keyword.
<br>
In the first function call 'baz();', the global variable $foo has the value 'bar', and so it is output via echo.
<br>
The function then assigns a new value of 'baz' to $foo.
<br>
The second call of 'baz();' echos the value of 'bar' and assigns 'baz' to $foo again.
<br>
The third call  of 'baz();' echos the value of 'bar' and assigns 'baz' to $foo again.
<br>

{% raw %}

<img src="https://github.com/joekingTheThird3/joekingTheThird3.github.io/blob/master/assets/28-09-2019-0376.png?raw=true">
{% endraw %}
The explanation on stackoverflow seems to be incorrect?


{{ site.time | date_to_string }}
