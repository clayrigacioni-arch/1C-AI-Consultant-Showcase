[English](README.md) | [Русский](README_RU.md) | **Azərbaycan dili**

# 1C:Enterprise üçün süni intellekt məsləhətçisi — v3

Süni intellekt məsləhətçisi təbii dildə verilən sorğular əsasında 1C-də analitik hesabatlar əldə etməyə kömək edir. **Azərbaycan və rus dillərində sorğular dəstəklənir.**

Layihə məhsulun **üçüncü versiyasına** çatıb. Hazırkı demo versiya 1C-nin standart hesabatlarından və məlumatların kompozisiyası sistemindən — SKD-dən istifadə edir.

## v3-də nə dəyişib?

Layihə analitik sorğuların yaradılması və nəticələrin ayrıca vizuallaşdırılması yanaşmasından standart hesabatların sazlanmasına keçib.

Süni intellekt istifadəçinin məqsədini və hesabat parametrlərini müəyyənləşdirir: dövr, qruplaşdırmalar, filtrlər və göstəricilər. Tətbiq bu parametrləri mövcud ssenarilər kataloqu üzrə yoxlayır və əvvəlcədən sazlanmış hesabat variantına tətbiq edir. Hesablamalar və nəticənin formalaşdırılması 1C vasitəsilə yerinə yetirilir.

Ssenarilərin vahid emal mexanizmi əlavə hesabatların qoşulması və sazlanması ilə həllin imkanlarını genişləndirməyə şərait yaradır.

## Demo versiyanın imkanları

- Müştərilər, məhsullar və təşkilatlar üzrə satışların təhlili.
- Təchizatçılar və məhsullar üzrə alışların təhlili.
- Anbarlar və məhsullar üzrə mal hərəkətinin təhlili.
- Mətn sorğusu əsasında hesabat parametrlərinin sazlanması.
- Azərbaycan və rus dillərində sorğuların emalı.

Sorğu nümunələri:

- «2024-cü il üzrə müştərilər və məhsullar üzrə satış gəlirini göstər».
- «2023-cü ildə təchizatçılar üzrə alışları göstər».
- «Anbarlar üzrə mal hərəkətini göstər».
- «Покажи выручку за 2024 год по клиентам и номенклатуре».

## Hazırkı vəziyyət

Mövcud imkanlar konkret bazada qoşulmuş hesabatlardan və sazlanmış variantlardan asılıdır. Sınaqlar, analitik ssenarilərin genişləndirilməsi və pul vəsaitlərinin hərəkəti üzrə hesabatların təkmilləşdirilməsi davam edir. Daha mürəkkəb analitik sorğuların dəstəklənməsi planlaşdırılır.

Texnologiyalar: 1C:Enterprise 8.3, BSL, SKD, standart hesabatlar, OpenAI API, HTTP/JSON.

Repozitoriyada layihənin açıq təsviri və nümayiş materialları yerləşdirilir. Mənbə kodu, quraşdırma faylları və süni intellektin daxili təlimatları yayımlanmır.

## v3 nümayişi: sorğu → hesabat

Demo bazadan götürülmüş ekran görüntüləri mətn sorğusunu və nəticədə formalaşan standart 1C hesabatını göstərir.

### Mal hərəkəti — Azərbaycan dilində sorğu

Sorğu: «anbarlar üzrə mal hərəkətini göstər 2023-cü il üzrə».

![Azərbaycan dilində mal hərəkəti sorğusu](screenshots/v3/warehouse-question-az.jpg)

Nəticə: 01.01.2023–31.12.2023 dövrü üzrə ilkin qalıq, mədaxil, məxaric və son qalığı göstərən anbar hesabatı.

![2023-cü il üzrə anbar hesabatı](screenshots/v3/warehouse-report.jpg)

### Alışların təhlili — rus dilində sorğu

2022-ci il üzrə təchizatçılar və məhsullar əsasında alış məbləğlərinin göstərilməsi barədə sorğu.

![Rus dilində alışların təhlili sorğusu](screenshots/v3/purchases-question-ru.jpg)

Nəticə: 01.01.2022–31.12.2022 dövrü üzrə təchizatçılar və məhsullar əsasında qruplaşdırılmış alış hesabatı.

![2022-ci il üzrə təchizatçılar və məhsullar əsasında alış hesabatı](screenshots/v3/purchases-report.jpg)

## Əvvəlki versiyaların ekran görüntüləri

Aşağıdakı şəkillər məhsulun əvvəlki versiyalarının interfeysini və vizuallaşdırma imkanlarını göstərir. Bunlar v3-ün ekran görüntüləri deyil. Materiallar demo bazada hazırlanıb.

![Əvvəlki versiyanın interfeysi](main-interface.jpg)

![Əvvəlki versiyada cədvəl](table-result.jpg)

![Əvvəlki versiyada diaqram](chart-result.jpg)

![Əvvəlki versiyada qrafik](graph-result.jpg)
