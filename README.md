## Readme for tutorial8 publisher repository
a. How many data your publlsher program will send to the message broker in one run? <br>
Jawab: Pada program publisher yang dibuat, diinisiasi broker CrosstownBus kemudian diterbitkan lima `UserCreatedEventMessage` menggunakan method publish_event pada file main.rs.
Jadi, dalam satu kali program dijalankan, publisher akan mengirimkan sebanyak 5 pesan data ke broker <br>
<br>
b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? <br>
Jawab: Pada publisher digunakan url yang sama dengan yang terdapat pada program subscriber karena url `amqp://guest:guest@localhost:5672` sejatinya merupakan link url yang biasa
digunakan untuk terhubung dengan message broker dengan menggunakan AMQP (Advanced Message Queuing Protocol). Ketika url yang sama digunakan pada publisher dan subscriber, maka kedua
program ini akan terhubung ke message broker pada mesin ,nomor kredensial hingga port yang sama. Hal ini akan memastikan bahwa penerbit dapat menerbitkan pesan ke contoh broker pesan 
yang sama dengan tempat pelanggan berlangganan
![alt text](<running rabbit.jpg>)
![alt text](<sending n processing.jpg>)
![alt text](<monitoring chart.jpg>)