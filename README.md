# Todo App

Bu proje, Go, Chi router ve Vue.js kullanarak yapılmış basit bir Todo uygulamasıdır. Kullanıcılar, öncelik seviyeleriyle todo oluşturabilir, görüntüleyebilir, güncelleyebilir ve silebilirler.

## Özellikler

- Başlık ve öncelik ile yeni todo oluşturma
- Tüm todoları görüntüleme ve önceliğe göre sıralama
- Todo başlığını, önceliğini ve tamamlanma durumunu güncelleme
- Todo silme
- Vue.js ve Bootstrap ile interaktif arayüz

## Kurulum

### Gereksinimler

- Go (sürüm 1.15+)
- Node.js (Vue.js geliştirmesi için)

### Backend Kurulumu

1. Depoyu klonlayın:

    ```bash
    git clone https://github.com/kullaniciadi/todo-app.git
    cd todo-app
    ```

2. Go bağımlılıklarını yükleyin:

    ```bash
    go mod download
    ```

3. Sunucuyu başlatın:

    ```bash
    go run main.go
    ```

    Sunucu `http://localhost:9000` adresinde çalışacaktır.

### Frontend Kurulumu

1. Vue.js ve ilgili bağımlılıkları yükleyin:

    ```bash
    npm install vue vue-resource
    ```

## Kullanım

### Uygulamaya Erişim

Tarayıcınızı açın ve `http://localhost:9000` adresine gidin.

### Todo Oluşturma

- Başlık ve öncelik girin.
- Ekle butonuna tıklayın.

### Todo Güncelleme

- Bir todo öğesine tıklayarak tamamlandı/tamamlanmadı yapın.
- Düzenle butonuna tıklayarak başlık veya önceliği güncelleyin.

### Todo Silme

- Sil butonuna tıklayarak bir todo öğesini silin.

## API Endpoints

### GET /todo

Tüm todoları getirir.

### POST /todo

Yeni bir todo oluşturur.

- **İstek Gövdesi:**
  ```json
  {
    "title": "Yeni Todo",
    "priority": 1
  }
