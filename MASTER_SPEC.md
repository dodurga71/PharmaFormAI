# PharmaForm AI — Master Spec

## Proje Özeti
PharmaForm AI, farmasötik teknoloji alanında formülasyon geliştirme, stabilite öngörüsü ve optimizasyon süreçlerini destekleyen AI tabanlı karar destek platformudur.

## Ana Amaç
Araştırmacıların deneme-yanılma yükünü azaltmak, daha doğru formülasyon başlangıç noktaları önermek ve Ar-Ge sürecini hızlandırmak.

## MVP Kapsamı
1. Etkin madde profil girişi
2. Formülasyon öneri motoru
3. Eksipiyan uyumluluk analizi
4. Stabilite risk puanlama
5. DoE / optimizasyon planlama
6. Salım kinetiği analizi
7. Otomatik raporlama

## Hedef Kullanıcılar
- Eczacılık fakültesi araştırmacıları
- Yüksek lisans / doktora öğrencileri
- Farmasötik teknoloji laboratuvarları
- Ar-Ge ekipleri
- İlaç / biyotek startup ekipleri

## İlk Ürün Stratejisi
İlk sürüm genel platform olmayacak.

İlk odak:
- nazal formülasyon
- hidrojel
- nanoformülasyon

## Temel Ürün İlkeleri
- açıklanabilir öneriler
- küçük ama sağlam MVP
- over-engineering yok
- modüler mimari
- veri geldikçe gelişen AI katmanı
- önce rule-based + yapılandırılmış mantık
- sonra ML / ileri AI

## Ana Modüller

### Backend
- proje yönetimi
- etkin madde verileri
- eksipiyan verileri
- analiz motorları
- raporlama

### Frontend
- dashboard
- proje oluşturma
- etkin madde formu
- öneri ekranı
- risk ekranı
- analiz ekranı
- rapor ekranı

### Intelligence Layer
- formulation recommender
- compatibility engine
- stability scoring engine
- DoE planner
- release kinetics analyzer
- reporting engine

## Teknoloji Yığını
- Backend: FastAPI
- Frontend: React
- Database: PostgreSQL
- Data/ML: Python, pandas, scikit-learn
- Optimization: scipy, optuna
- Visualization: plotly / matplotlib

## Çalışma Prensibi
- önce mimari
- sonra veri modeli
- sonra backend iskeleti
- sonra frontend iskeleti
- sonra çekirdek motorlar
- sonra Codex görev zinciri
- sonra MVP teslimi

## Başarı Ölçütleri
- ilk deneme kalitesinin artması
- gereksiz deney sayısının azalması
- raporlama süresinin kısalması
- açıklanabilir karar üretimi
- sürdürülebilir mimari
