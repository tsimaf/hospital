﻿# hospital

Для использования всех возможностей Jupyter Notebook проект рекомендуется открывать в nbviewer:
[nbviewer](https://nbviewer.org/github/tsimaf/hospital/blob/c29a11e2da52b167f00d05a52e9e7c55763e1396/hospital.ipynb)

Открыть ipynb внутри GitHub:
[ipynb](https://github.com/tsimaf/hospital/blob/main/hospital.ipynb)

Отчет в DataLens:
[DataLens](https://datalens.yandex/yuiiscqzr0xul)

## Задачи проекта
Заказчик - Педиатрический Университет. На основании данных о госпитализации пациентов медицинского центра рассчитать длительность в днях, прошедших от выдачи направления до поступления пациента в медицинский центр, определить, что влияет на длительность. Предоставить всю возможную информацию по диагнозам: срок лечения, время в ожидании, прочие факторы. Провести Ad-hoc исследование данных. А также подготовить отчет в BI-системе.

## Навыки и инструменты
- Python
- PostgreSQL
- DataLens
- Ad-hoc исследование
- Pandas
- Matplotlib
- Seaborn
- Ydata_profiling
- Phik
- Scipy.stats
- Проверка статистических гипотез

## Выводы
В ходе работы загрузил данные с сервера PostgreSQL, провел предобработку данных, рассчитал длительность в днях, прошедших от выдачи направления до поступления пациента в медицинский центр, провел разведочный анализ данных при помощи библиотеки ydata_profiling, провел исследовательский анализ данных, провел аналитическую работу, определил факторы, влияющие на время поступления пациента, провел проверку на наличие корреляции при помощи библиотеки phik, сформировал и проверил гипотезы, подготовил отчет в BI-системе DataLens, сформулировал выводы и предложил следующие рекомендации заказчику:
- Исходя из того, что наибольшее влияние на количество дней ожидания госпитализации и на другие факторы оказывает диагноз при выписке пациента из госпиталя, рекомендуется приложить все усилия, чтобы минимизировать ошибку при первичной постановке диагноза пациента.
- Наблюдается высокая задержка по госпитализации пациентов проходящих через плательщика ОМС 86 Регион (а это 40% от всех пациентов и динамика продолжает расти). Этот момент рекомендуется обсудить на уровне плательщика. Возможно, есть способы скорректировать процесс регистрации и оплаты для пациентов, поступающих через ОМС 86 Регион.
- При записи пациентов в базу, попадающих в госпиталь через скорую помощь и другие экстренные случаи, при возможности рекомендуется минимизировать пропуски в графах с датой выдачи направления и регионом для более глубокого анализа времени ожидания пациентами госпитализации.
- Для оценки заполняемости отделений, а также для дальнейшего прогнозирования и корректировки количества мест в отделениях, рекомендуется предоставить данные о количестве койко-мест в отделениях госпиталя.
