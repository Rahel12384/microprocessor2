# نام آزمایش :

روشن کردن LED با 'H'یا 'h' و خاموش کردن LED با 'L' یا 'l'

## هدف آزمایش :

روشن کردن LED با سریال مانیتور با استفاده از کدهای تعریفی L & H یا h & l توسط کاربر 

## ابزار مورد نیاز :

* 1 برد آردوینو
  
* 2 یک عدد LED
  
* 3 مقاومت
  
* 4 سیم‌های رابط
  
* 5 کابل اتصال USB به کامپیوتر
  

## شرح آزمایش :

  * 1 ابتدا LED را روی برد بورد قرار میدهیم.
  * 2 مقاومت 220 اهمی را به سر منفی (کاتد ، کوتاه تر) وصل میکنیم.
  * 3 سر دیگر مقاومت را به Gnd بورد آردینو (زمین) وصل میکنیم.
  * 4 پایه مثبت (آند ، بلندتر) LED را به پایه شماره 13 بورد آردینو وصل میکنیم.
  * 5 بورد اردینو را توسط کابل  USB  به کامپیوتر وصل میکنیم.


## کد آزمایش :

const int led = 13;

void setup()

{

pinMode(led , OUTPUT);

Serial.begin(9600);

}

void loop() 

{

if(Serial.available()>0)

{

  char incomingByte = Serial.read();
  
  if(incomingByte == 'H' || incomingByte == 'h')
  
  {
  
  digitalWrite(led , HIGH);
    
  }
  
  else if(incomingByte == 'L' || incomingByte == 'l')
  
  {
  
  digitalWrite(led , Low);
  }
  
}

}

## نتیجه گیری: 
اگر کاربر حرف H یا h را وارد کند LED روشن میشود و اگر کاربر حرف L یا l را وارد کند LED خاموش میشود

## شکل مدار
![توضیح تصویر](https://github.com/Rahel12384/microprocessor-2/blob/main/Micro3/Report%201/IMG_20241007_103823.jpg)

![توضیح تصویر](https://github.com/Rahel12384/microprocessor-2/blob/main/Micro3/Report%201/IMG_20241007_103832.jpg)


