# Monitoring Real-Time Warehouse Conditions with Apache Kafka & PySpark
#### A streaming analytics project to monitor temperature and humidity across multiple warehouses in real‑time. Utilizes Dockerized Apache Kafka for ingestion, a Python-based producer for sensor simulation, and PySpark Structured Streaming for processing and alert generation.

## Overview
### Perusahaan logistik membutuhkan pemantauan suhu dan kelembaban di gudang yang menyimpan barang sensitif (makanan, obat‑obatan, elektronik).  
#### Mensimulasikan data sensor secara real‑time via Python producer (data.py).

#### Menyajikan data ke topik Kafka: sensor-suhu-gudang & sensor-kelembapan-gudang.

#### Memproses stream di PySpark (consumer.py), menggabungkan windowed streams, dan menghasilkan status:

##### Aman
##### Suhu tinggi, kelembaban normal
##### Kelembaban tinggi, suhu aman
##### Bahaya tinggi! Barang berisiko rusak
