
## Описание на проекта

Този проект демонстрира конфигурацията и деплоймента на услуга с помощта на Kubernetes и Flux CD. Услугата използва контейнер с приложението **Podinfo** и е настроена да се деплойва автоматично чрез Flux.

## Структура на проекта

Проектът съдържа следните основни директории и файлове:

- `deploy/`: Конфигурационни файлове за деплоймента на Podinfo.
  - `podinfo-configmap.yaml`: Конфигурационен файл за PodInfo.
  - `podinfo-deployment.yaml`: Конфигурация на деплоймента.
  - `podinfo-secret.yaml`: Конфигурационен файл за секрети.
  - `podinfo-service.yaml`: Конфигурационен файл за услугата (Service).

- `podinfo/`: Конфигурации, свързани с Flux и Kubernetes.
  - `GitRepository.yaml`: Конфигурация за Flux GitRepository.
  - `deployment.yaml`: Конфигурация на деплоймента на PodInfo.
  - `flux-kustomization.yaml`: Конфигурация на Flux Kustomization.
  - `podinfo-deployment.yaml`: Конфигурация на PodInfo като деплоймент.
  - `podinfo.yaml`: Основни YAML конфигурации за PodInfo.
  - `service.yaml`: Конфигурация на услугата PodInfo.

- `podinfo-repo/`: Ресурси, свързани с репозитория на PodInfo.

## Изисквания

- **Kubernetes Cluster**: Работещ Kubernetes клъстер.
- **Flux CD**: Инсталиран Flux CD за управление на Kubernetes ресурсите.
- **Kubectl**: Команден инструмент за взаимодействие с Kubernetes.
- **Git**: Репозитория за конфигурации в Git.