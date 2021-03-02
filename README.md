# TalkingRobotHeadProject
## Konuşan Robot Kafa (MyrobotLab ve Arduino) 

<p align="center">
  <img width="518" height="345" src="https://github.com/celikslab/TalkingRobotHead/blob/main/%C4%B0mages/robot.JPG">
</p>

<br>İnsansı robot, vücut şekli insan vücuduna benzemek üzere üretilen robottur. İnsan vücudunu taklit etmeye çalışmak onu daha iyi anlamayı sağlamaktadır. Bu projede insanın konuşmayı algılaması ve ses-konuşma üretmesi taklit edilmiştir. Projenin amacı ses komutlarını algılayıp, bu komutlara karşılık gelen fonksiyonları gerçekleştirebilen bir robotun yapılmasıdır. Bunun için yapay zekanın alt dallarından olan ses sentezleme ve ses tanıma kullanılmıştır. Robotun gelen ses sinyallerini sayısal değerlere sonrasında ise yazıya dönüştürmesinde ses-konuşma tanıma, cevap üretip konuşabilmesini sağlamak için de ses sinyallerini sayısal değerlere çevirebilmesi için ise ses-konuşma üretme sisteminden yararlanılmıştır.</li>

## Kullanılan Malzemeler

<li>Mg996R Servo Motor x 2 adet</li>
<li>Sg-90 Servo Motor x 3 adet</li>
<li>Arduino Uno R3 Mikrodenetleyici</li>
<li>Windows Tabanlı Bilgisayar</li>
<li>5mm Led x 2 adet </li>
<li>220Ohm Direnç x 2 adet</li>
<li>12Volt 5Amper Trafo </li>
<li>Lm2596 Voltaj Regülatör Modülü (12v to 5v)</li>
<li>608zz Rulman x 2 adet</li>
<li>Dişi-dişi, Dişi-erkek Jumper Kablo</li>
<li>Tda2030 amfi Modülü</li>
<li>8Ohm 5W Mini Hoparlör</li>
<li>Mikrofon</li>
<li>Erkek Jack</li>
<li>3mm Vidalar</li>
<li>2mm Çaplı Bükülebilir Tel</li>


## Devre Şeması

<p align="center">
  <img width="518" height="345" src="https://github.com/celikslab/TalkingRobotHead/blob/main/%C4%B0mages/CircuitSchematic.png">
</p>



## 3D Baskı

3D yazıcılar, eklemeli olarak yani malzemeyi katman katman ekleyerek istenilen parçayı oluştururlar. Bu yöntem, geleneksel imalat yöntemlerine karşın birçok avantaj sunsada, şu anda, 3D yazıcıların geleneksel imalat yöntemlerinin çoğunun yerini doldurması pek olası değildir. Ancak 3D yazıcıların işlevsel bir malzeme ile yüksek doğruluk ve hızla kullanılabilecekleri birçok uygulama vardır. Bu projede de kolay ve hızlı üretim, düşük maliyet ve uygunluk(karmaşık yüzey üretimi, malzeme hafifliği) gibi birçok avantajından ötürü 3d yazıcı ile üretim tercih edilmiştir.

<p align="center">
  <img width="533" height="287" src="https://github.com/celikslab/TalkingRobotHead/blob/main/%C4%B0mages/cura.PNG">
</p>

Çizim dosyalarına(stl) [buradan](https://github.com/celikslab/TalkingRobotHead/tree/main/stl) ulaşabilirsiniz.

Baskı Ayarları :

<li>İnfill: %30</li>
<li>Resolution: 0.2</li>
<li>Speed: 60 mm/s</li>
<li>Support: Yes</li>
<li>Filament material: Pla+ Purple-White</li>

## Montaj

Bu robot prototipi kafa, boyun, stand olarak 3 ayrı kısımdan oluşmaktadır. Montaja ilk olarak kafa kısmının iskelet yapısı birleştirilerek küçük(sg90) ve büyük(mg996) servo motorlar yuvalarına montajlandı. Ardından gözlerin yataklara montajı yapıldı. Küçük servo motorlar(sg90), gözlere ince bakır tel ile bağlandı çünkü bakır teller bir şaft görevi görerek servo motorlar dönerken gözleri x ve y ekseninde hareketini gerçekleştirir. Burada unutulmaması gereken şey ise bakır teller(şaftlar), servolara bağlanacak kısımları servoların ve eksenin kalibrasyonu yapıldıktan sonra takılmalıdır! Boyun kısmına gelirsek kafayı y ekseninde hareket ettirecek parçalar eklem yerine rulman yerleştirilerek kafaya bağlandı ve kafada bulunan y ekseni hareketini sağlayacak servoya şaft takıldı. Daha alt kısımda x ekseni hareketinin sağlanması için tutucuya servo motor sabitlenerek tutucunun merkezine rulman yerleştirildi. Sonra çene takıldı ve ilgili servoya şaft ile bağlantısı yapıldı. Yüzü oluşturan plakalar takıldı. Tutucu kısımda kutu şeklindeki standa montajlandı. Kablolar bir kablo kanalından geçirilerek standın içerisine ulaştırıldı. Standın içerisine Arduino ,regülatör ,amfi kartları bağlantıları yapılarak yerleştirildi ve standın kapağı kapatıldı.

<p align="center">
  <img width="615" height="310" src="https://github.com/celikslab/TalkingRobotHead/blob/main/%C4%B0mages/design.png">
</p>

## Kodlar
