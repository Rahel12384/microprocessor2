# نام آزمایش :
دستور begin


## هدف :
ارسال یک پیام از طریق ارتباط سریال

 
  ## کد آزمایش :

void setup() 

{

serial.begin(9600);

}

void loop() 

{
 
serial.print("hello raheleh!")

delay(1000);

}


  ## توضیحات کد  :
  serial.begin(9600) : سرعت ارتباط سریال ۹۶۰۰ است.

  serial.print("hello raheleh!"): ارسال پیام از طریق ارتباط سریال .

  delay(1000): وقفه ۱ ثانیه ای


##نتیجه گیری:

این برنامه هر ۱ ثانیه دستور hello raheleh را چاپ میکند

نکته: اگر حرف ln را بعد از کلمه print  بنویسیم ، هرکدام از این دستورات در خط های پشت سر هم چاپ میشوند
درغیر این صورت همه پشت سر هم چاپ میشود

## شماتیک مدار
![توضیح تصویر]()
 
  