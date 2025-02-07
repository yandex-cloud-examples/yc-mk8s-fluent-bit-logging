# Отправка логов кластера Yandex Managed Service for Kubernetes® в Yandex Cloud Logging с помощью Fluent Bit

С помощью [Fluent Bit](https://fluentbit.io) вы можете транслировать логи подов и сервисов [Managed Service for Kubernetes®](https://yandex.cloud/ru/docs/managed-kubernetes) в [Cloud Logging](https://yandex.cloud/ru/docs/logging). Установка и настройка Fluent Bit описана в [практическом руководстве](https://cloud.yandex.ru/ru/docs/managed-kubernetes/tutorials/fluent-bit-logging)

В этом репозитории расположены конфигурационные файлы:

* [k8s-cluster-with-log-group.tf](k8s-cluster-with-log-group.tf) — для создания инфраструктуры для Managed Service for Kubernetes® и Cloud Logging через Terraform.
* [systemd.yaml](systemd.yaml) — для установки Fluent Bit через Helm.
* [config.yaml](config.yaml) — для установки Fluent Bit вручную.
