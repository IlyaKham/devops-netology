# Gitignore для проекта

Добавленные файлы .gitignore будут игнорировать следующие типы файлов:

## В terraform/.gitignore:
- Директорию .terraform/ с плагинами и кэшем
- Файлы состояний Terraform (*.tfstate, *.tfstate.backup)
- Файлы переменных с чувствительными данными (*.tfvars)
- Файлы блокировки состояний (.terraform.tfstate.lock.info)
- Crash-логи (crash.log)
- Файлы переопределения (override.tf, override.tf.json)
