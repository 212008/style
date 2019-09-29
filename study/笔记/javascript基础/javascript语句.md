# 第五章 JavaScript语句
### 5.1 分支语句
5.1.1 if 语句

		var a = 10;
        //小括号里一定要是true
        if(a<20){
            alert('yes')
        }

5.1.2 if...else...

        if(a<20){
            alert('yes')
        }else{
            alert('no')
        }

5.1.3 if...else if...
 
		if(a<60){
            alert('D');
        }else if(a>=60 && a<75){
            alert('C');
        }else if(a>=75 && a<85){
            alert('B');
        }else if(a>=85 && a<=100){
            alert('A');
        }else{
            alert('缺考');
        }

5.1.4 switch语句
switch小括号中一般情况是一个变量名,这个变量可能会有不同的取值.所有的case都是"或"的关系,case后面的值会与变量值作比对,满足后就执行case后面的代码.不写break就会将所有的比较进行一遍.

		var a = 10;
        //将判断的内容写在括号里
        switch(a){
            case 值1:
            //执行代码
            break;
            case 值2:
            //执行代码
            break;
            case 值3:
            //执行代码
            break;
            case 值n:
            //执行代码
            break;
            default:
            //执行代码
        }

###5.2 循环语句
5.2.1 while循环
while语句是一种前测试语句(先判断一下在执行),循环的目的是为了反复执行语句或代码块,只要表达式为true就继续循环,一旦为假的时候,循环退出.

		//先找一个变量接住计算的和,最开始是0
        var sum = 0;
        //我要做一大堆我现在还不会的事情
        //范围是1~<=10
        var a = 1;
        //我需要一个循环来让我的a++ 一直到 <=10
        while(a<=10){
            sum += a;  //累加专用(套路)
            a++;
        }

5.2.2 do....while循环
do...while语句是一种后测试语句,就是在循环体中的代码执行之后,才开始判断条件.也就是说,在表达式判断之前,循环体内的代码至少会被执行一次.

        var a = 0;
        do{
            alert('nihao');
            a++;
        }while(a<5)

5.2.3 for循环

for语句是一种前测试语句,一般情况下,有三个基础表达式语句,每一个要用分号隔开.

		for(var i = 0;i<=5;i++){
            for(var z = 0;z<=5;z++){
                document.write('❤');
            }
            document.write('<br>');
        }
		//顺序为:初始化-->判断 执行循环体 -->更新






##练习
需求
1.做一个1+2+3+4+5+6+7+8+9+10的和