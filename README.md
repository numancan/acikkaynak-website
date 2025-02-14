# [acikkaynak-website](https://github.com/acikkaynak/acikkaynak-website)

[![derleme durumu][build-image]][build-url]
[![bağımlılıklar][dep-image]][dep-url]
[![kapsam durumu][coverage-image]][coverage-url]
[![lisans][license-image]][license-url]

## BENİ OKU

Bu kod tabanında, şu anda yapım aşamasında bulunan [acikkaynak.info](https://preview.acikkaynak.info/)'nun önizleme sürümü yer almaktadır.

`master` branch'ine aktarılan değişiklikler, bir dizi derleme işleminden sonra [https://preview.acikkaynak.info/](https://preview.acikkaynak.info/)
adresinde belirecektir. Henüz buradaki değişiklikler `acikkaynak.info` adresindeki yayını etkilememektedir.


## Katkı Sağlamak

### Çalışma Ortamını Hazırlamak

`node.js`'in ve `yarn`'ın sisteminizde kurulu olduğundan emin olun.

Repository'i klonlayıp, npm üzerinden bağımlılıkları çekerek çalışma ortamınızı hazır hale getirin.

```sh
git clone https://github.com/acikkaynak/acikkaynak-website.git
cd acikkaynak-website
yarn install
yarn dev
```

### Çalışmaya Başlamak

`yarn dev` komutu ile geliştirme modunda kod tabanına müdahale etmeye başlayabilirsiniz. Komutu çalıştırdıktan bir süre
sonra browser'ınız açılacak, siz değişiklik yaptığınız sürece "hot reloading" sayesinde browser'daki kod otomatik olarak
güncellenecektir.


### Çalışmayı Kontrol Etmek

`yarn lint` komutu ile yazılan kodun belirlenen eslint standartlarına uyup uymadığını kontrol edebilirsiniz. Eğer bu
kontrolü yapmazsanız Pull Request oluşturduğunuzda GitHub tarafından bu kontroller otomatik işletilecek ve açmış olduğunuz
Pull Request'i sizden güncellemenizi isteyecektir.

Bazı kod standartları otomatik olarak düzeltilebilmektedir, bunu sağlamak için `yarn lint:fix` komutunu kullanabilirsiniz.

Aynı zamanda yazmış olduğunuz birim testlerini `yarn test` komutu ile başlatabilirsiniz. Testler de aynı lint işlemi gibi
hem pull request hem de push esnasında GitHub Actions tarafından CI/CD otomasyonuna bağlı olarak çalıştırılmaktadır.


## Dizin Yapısı

| Klasör                                          | Açıklama                                                        |
|-------------------------------------------------|-----------------------------------------------------------------|
| `/src/`                                         | Kaynak dosyalarını içeren klasör                                |
| `/src/app/`                                     | Ana uygulama kaynak kodları                                     |
| `/src/app/layouts/default/`                     | - Varsayılan tema                                               |
| `/src/app/layouts/default/assets/`              | - Varsayılan temanın assetleri (resim, font, stiller, v.b.)     |
| `/src/app/layouts/shared/assets/`               | - Tüm temaların ortak assetleri (resim, font, stiller, v.b.)    |
| `/src/app/pages/`                               | - Sayfalar ve sayfalara ait React bileşenleri                   |
| `/src/app/app.tsx`                              | - Uygulamanın router noktası                                    |
| `/src/startup.ts`                               | Tüm uygulama için bağımlılık bağlantıları ve konfigurasyon      |
| `/src/index.html`                               | HTML Şablonu                                                    |
| `/semantic-ui/`                                 | Semantic UI'a ait tema ve site özelleştirme yapısı              |
| `/public/`                                      | Web dizininde yer alacak tüm statik dosyalar                    |


## Yapılacaklar

[GitHub Projesi](https://github.com/orgs/acikkaynak/projects/1) üzerinde detaylar yer almaktadır.


## Gereksinimler

* node.js (https://nodejs.org/)


## Notlar ve Teşekkürler

Webfontları içeri gömmek için [google-webfonts-helper](https://google-webfonts-helper.herokuapp.com/) kullanılmaktadır.


## Lisans

Apache 2.0, daha fazla detay için lütfen [LICENSE](LICENSE) dosyasını inceleyin.


## Katkı Sağlayanlar

[contributors.md](contributors.md) dosyasını inceleyebilirsiniz.

Herhangi bir katkıya açıktır. Hata düzenlemeleri, yeni özellik ve modüller ekleyebilirsiniz.

* Koda katkı sağlamak için: Yukarıda anlatıldığı gibi repository'i klonlayın, değişikliklerinizi gerçekleştirin, ve bir pull request oluşturun.
* Bir hata bildirmek için: Bir şeyler ters gidiyorsa, [GitHub Issues](https://github.com/acikkaynak/acikkaynak-website/issues) üzerinden yeni bir issue oluşturup bize bildirin.


[build-image]: https://github.com/acikkaynak/acikkaynak-website/workflows/CI/badge.svg
[build-url]: https://github.com/acikkaynak/acikkaynak-website/actions?workflow=CI
[dep-image]: https://img.shields.io/david/acikkaynak/acikkaynak-website.svg?style=flat-square
[dep-url]: https://github.com/acikkaynak/acikkaynak-website
[coverage-image]: https://img.shields.io/codecov/c/gh/acikkaynak/acikkaynak-website/master.svg?style=flat-square
[coverage-url]: https://codecov.io/gh/acikkaynak/acikkaynak-website
[license-image]: https://img.shields.io/github/license/acikkaynak/acikkaynak-website.svg?style=flat-square
[license-url]: https://github.com/acikkaynak/acikkaynak-website/blob/master/LICENSE
