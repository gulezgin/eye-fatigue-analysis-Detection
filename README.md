# eye-fatigue-analysis-Detection
This project is an eye blink detection application used to detect fatigue by tracking eye movements in a video stream.

Göz Kırpma Tespiti ve Yorgunluk Algılama
Bu proje, video akışında göz kırpma hareketlerini izleyerek kullanıcıların yorgunluğunu algılayan bir uygulamadır. Gözün kapanma oranını (Eye Aspect Ratio, EAR) kullanarak yorgunluğu tespit eder ve ekran üzerinde bir uyarı gösterir.

Özellikler
Yüz ve göz algılama
Göz kapanma oranını (EAR) hesaplama
Yorgunluk tespiti için bir eşik değeri belirleme
Ekranda yorgunluk uyarısı gösterme
Gereksinimler
Python 3.x
OpenCV
dlib
numpy
scipy
Gerekli Python paketlerini yüklemek için:

bash
Copy code
pip install opencv-python dlib numpy scipy
Kurulum
Dlib'in Yüz Nokta Modelini İndirin:

shape_predictor_68_face_landmarks.dat dosyasını dlib.net adresinden indirin ve proje klasörüne yerleştirin.

Kodunuzu Çalıştırın:

Aşağıdaki komutu kullanarak Python scriptinizi çalıştırın:

bash
Copy code
python main.py
Kod Açıklaması
calculate_ear(eye): Bir gözün kapanma oranını hesaplar.
draw_eye_landmarks(frame, eye_landmarks): Göz üzerindeki önemli noktaları ekranda işaretler.
main(): Video akışını başlatır, yüz ve gözleri tespit eder, EAR hesaplar ve yorgunluk uyarısını gösterir.
Kullanım
Uygulamayı başlattıktan sonra, web kamerası ile görüntü alınır.
Gözlerinizin kapanma oranı izlenir ve belirlenen eşik değeri altında olduğunda "YORGUNLUK ALGILANDI!" mesajı ekranda görüntülenir.
Programdan çıkmak için q tuşuna basın.
Sorun Giderme
shape_predictor_68_face_landmarks.dat dosyasının doğru yerde olduğundan emin olun.
Kamera erişimi izinlerini kontrol edin ve başka uygulamaların kamerayı kullanmadığından emin olun.
Katkıda Bulunma
Bu projeye katkıda bulunmak isterseniz, pull request göndererek veya açık sorunları çözerek yardımcı olabilirsiniz.
