# Нейросетевые технологии, лабораторная работа №4 "Изучение RNN на примере научной статьи"

## Основа работы

[Применение LSTM-модели к прогнозированию СPI и уровня инфляции на примере России](https://1economic.ru/lib/114845)

## Источники данных
[Инфляция ЕМИСС](https://www.fedstat.ru/indicator/31074)

[Росстат — Цены, инфляция](https://rosstat.gov.ru/statistics/price)

[Исходный XLSX-файл](https://rosstat.gov.ru/storage/mediabank/ipc_mes_09-2026.xlsx)

## Структура проекта

| Директория | Назначение |
| --- | --- |
| docs/papers | Научные статьи |
| notebooks | Jupyter-ноутбуки |
| data/raw | Исходные данные |
| data/processed | Производные данные |

## Развёртывание окружения

В Miniforge Prompt
```bash
conda init powershell
```

В терминале
```bash
conda env create -f environment.yml
conda activate fourth_lab

dvc remote modify local_storage url /pat/to/dvc-storage
dvc pull

nbstripout --install
```