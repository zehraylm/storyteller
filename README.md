# storyteller
Yapay zeka kullanarak kendi kendine hikaye kitabı oluşturabilen bir program oluşturmaya çalışırken nasıl adımlar izlendiği açıklanmıştır.

## Hikaye Oluşturmak
Bu kısımda chatGpt kullanılarak bize kısa ingilizce bir hikaye anlatmasını istiyoruz.

## Hikaye Bileşenleri
Bu kısımda resim çizdirilirken kullanılacak olan temel bileşenleri elde etmeye çalışıyoruz. Öncelikle hikayedeki kişileri çıkartabilmek için chatGpt'ye hikayede bulunan kişileri tanımlamasını istiyoruz. Ardından hikayeyi sayfalara bölmemiz gerekiyor bunun için de hikayeyi önce paragraflar bazında ele alıyoruz. Bu aşamada ele alınan paragrafları Chatgpt'ye verip bu metni birkaç kelime ile ingilizce tanımla diyoruz. Böylece elimizde paragrafta geçen olayın birkaç kelimelik özeti oluyor. Ardından bu özette elimizde bulunan karakter tanımlamalarını da isimleri yerine yazıyoruz.
Böylece hikaye kitabında sayfa için resim promptu temeli oluşmuş oluyor.

## Hikaye Resim Promptları
Bu aşamada ise hikaye bileşenlerinden elde ettiğimiz temel promptları ayrı ayrı ele alıp eklemeler yapıyoruz. Şimdiye kadar olan promptlarda sadece içerik ile ilgili bilgiler vardı. Ancak biz bir hikaye kitabı istiyorsak belli bir stilde resimler elde etmeliyiz. Ayrıca resimlerin bozuk çıkmaması için de ek parametreler eklememiz gerekir. 
Bundan yola çıkarak;
Hikaye özet promptu + Stil promptları + diğer pozitif promptlar 
şeklinde resim çıktısı için olan promptu oluşturmuş oluyoruz.

Şimdiye kadar genellikle kullandığım ek promptlar şu şekilde:

"Özet Prompt" + beautifull eyes, perfect face, intricate, elegant, highly detailed, digital painting, artstation, concept art, sharp focus, illustration, by justin gerard and artgerm, 8 k, centered,

Negatif Prompt için ise:

deformed, ugly, mutilated, disfigured, text, extra limbs, face cut, head cut, extra fingers, extra arms, poorly drawn face, mutation, bad proportions, cropped head, malformed limbs, mutated hands, fused fingers, long neck, deformed face,
şeklinde promptlar kullanıyorum.

## Sonuç 
Oluşturulan resim ve paragraflar page.html dosyasındaki alanlara yerleştiriliyor ve hikaye kitabı web arayüzünde görüntülemeye hazır hale geliyor.
Şimdiki halinde otomatik olarak kitap oluşturulamamaktadır. Chatgpt ve StableDiffusion kullanılarak bu adımlar izlendiği takdirde örnekteki gibi çıktılar elde edilebilmektedir.  
