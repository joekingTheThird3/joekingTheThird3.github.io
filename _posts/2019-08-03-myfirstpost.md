---
layout: post
title: "joekingthethird3 Launches Site"
date: 2019-08-03
salute: hello
---

data = site.data = {{  site.data }}
<br>
site.data.default = {{site.data.default}}
<br>
site.data.default.myvar = {{site.data.default.myvar}}

finally! {{  page.salute }}

Thanks to this guide on how to create a site on github  - <http://jmcglone.com/guides/github-pages/>

1. takes 2mins to update site/files on this github - annoyance
2. varibles in front matter - yaml - need prefix with page - e.g. page.salute 
3. blog directory in other repository interfered with this repository
4. _config.yml file had incorrect format - spaces infront of keys/variables - showed up as red bar
but only hint that there was a problem was in the settings tab of the repository. Ah! Actually I got an email with the error 'You have an error on line 2 of your `_config.yml` file'
5. What version of Jekyll am I using on github? Look at <https://pages.github.com/versions/> - v3.8.5 as of 05/08/2019




<br>
{{ site.time | date_to_string }}
