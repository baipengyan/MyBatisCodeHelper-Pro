# 无法进行激活
## 如果激活报密文数据已损坏或者DnsFilter.testQuery报错
请先更新到插件3.0.5(qq群:685465570)版本重新激活一下 如果还有问题，再看下面的   
请检查Intellij是否使用了ja-netfilter>=20220701版本   
最新版的ja-netfilter屏蔽了brucege.com并且不让插件进行正版验证 请打开ja-netfilter目录修改ja-netfilter\config\dns.conf  
把equal brucege.com 那一行给删掉   
并且还需修改ja-netfilter\config\power.conf  
请删除掉最后一行  
EQUAL,65537,112990544699464667379805164176191940546242208117491544203358534026745357579006792084392734842374059845912387257283707238075863959850326589016727302942528968334782467185179054600102556548201786183972872728459057873984508534595649484729912852626347880177196897414735118804133099744542685440257890337513274043513->3,112990544699464667379805164176191940546242208117491544203358534026745357579006792084392734842374059845912387257283707238075863959850326589016727302942528968334782467185179054600102556548201786183972872728459057873984508534595649484729912852626347880177196897414735118804133099744542685440257890337513274043513
然后重启idea即可正常激活  


## 如果电脑无法访问 http://brucege.com/pay/view
请联系微信gejun12311来进行离线激活，将插件离线激活里面的唯一码和购买的在线激活码发给他

## mac无法激活，Permission denied
![noPermission](https://myimages.brucege.com/noPermission.png)
请使用 cd ~ 然后 sudo chmod 777 .config 即可