# UrbanSoundClassification

## Preprocessing
Bu aşamada benden istenileceği gibi Grayscale,Resizing ve Normalizasyon işlemlerini gerçekleştireceğim fakat daha öncesinde Train ve Val olarak klasörleme yapmam gerekiyor bunun için kod içerisinde imagelist bölümünde bir index_list oluşturuyorum ve bu listeyi random.shuffle ile karıştırıyorum ve train val ve test olarak bölüyorum ve dosyalama yapıyrum fakat küçük bir sorunla karşılaşıyorum istediğim gibi eşit bir bölme yapamamışım. Bu yüzden test içerisindeki dosyaları val içerisine aktarıyorum ve val olarak val_gen içerisinde validation_split atarak test kümesini oluşturuyorum ve ImageDataGenerator bölümünde grayscale,resizing ve Normalizasyon işlemlerini gerçekleştiriyorum.


## Build Model 
Model oluşturma aşamasında basit bir model oluşturup istediğim bir sonuç yani underfitting olayını görürsem modeli karmaşıklaştırmayı düşünüyorum. Bu sayede son olarak oluşturduğum modelde kalıyorum. Epoch sayısı 50 ve eğer overfittinge gitme durumunu inceledim daha sonrasında gimediğini gördüğümde callbaks olarak earlystop'a ihtiyaç duymuyorum.

## Training
 Eğitim aşamasında loss değerleri birbirlerinden aşırı faklı yani arasındaki skala çok artmadığını gördüğüm için modeli böyle bırakıyorum ve test verisetiyle değerlendirmelerimi yapıyorum sonuç olarak projeyi burada bitiriyorum.

