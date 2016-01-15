## 排错

####排错流程：</br>
1. 确认JS已经触发 (第一行写alert(1);)</br>
2. 确认JS已经获取所有所需参数（每一个都需要打出来，用console.log是在浏览器的console里查看)</br>
3. 确认AJAX已经进入，注意AJAX传的第四个参数语法，是否少写"&"</br>
4. 确认mainserver里的URL及dao层方法调用正确</br>
5. 确认DAO层已经进入(DAO第一行打console.log("进入xxx DAO");	//在服务器控制台上查看</br>
6. 确认DAO层已经获取到所有AJAX传进来的参数 （每一个都需要打出来，用console.log)</br>
7. 打印DAO层返回的data</br>
8. data没有正确显示==> 在sqlyog里测试sql语句是否正确</br>
9. data有反应显示但是数据库没有更新 ==> 留意data返回的内容是否正确，在sqlyog里测试sql语句是否正确</br>
10. data正确显示，数据库已更新，但页面没有反应 ==> 浏览器是否报错，一般都是innerHTML语句错误，留意单双引号</br>
