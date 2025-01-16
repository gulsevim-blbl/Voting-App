# Kubernetes Voting App #
Bu proje, Kubernetes kullanarak basit bir oylama uygulamasını çalıştırır. Uygulama, Vote (oylama) ve Result (sonuç) bileşenlerini içerir. Redis, PostgreSQL ve Worker bileşenleri arka planda çalışır.

## Kurulum Adımları
Projeyi Klonlayın:

```bash
git clone https://github.com/YOUR_USERNAME/voting-app.git
cd voting-app
```
```bash
Namespace
kubectl create namespace voting-app
```
```bash
Deployment Dosyalarını Uygulayın:
kubectl apply -f deployments/
```
```bash
Servislere Erişin:
Vote ve Result servislerini görmek için:
kubectl get svc

Minikube kullanıyorsanız:
minikube service vote
minikube service result
```

## Bileşenler!
Vote App: Oy verme arayüzü.
Result App: Gerçek zamanlı sonuç gösterimi.
Redis: Oyların geçici saklanması.
PostgreSQL: Veritabanı.
Worker: Oyların işlenmesi.
