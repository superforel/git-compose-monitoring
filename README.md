Первым делом что нужно сделать это прописать:
- git clone https://github.com/superforel/git-compose-monitoring.git

Наш репозиторий содержит два файла docker-compose.yml для разделения логики приложения. Первый файл определяет сервисы backend и frontend (WordPress), обеспечивая их запуск. Второй файл описывает сервисы мониторинга: экспортеры метрик и базу данных Prometheus. После запуска этих сервисов, подключение к Grafana по порту 3000 и использование соответствующих дашбордов позволяет визуализировать состояние системы и отдельных микросервисов в виде графиков и диаграмм.

Для запуска и остановки сервисов, описанных в файлах Docker Compose, необходимо установить утилиту make (команда sudo apt install make). Запуск осуществляется командой make compose-up, а остановка — командой make compose-down.
