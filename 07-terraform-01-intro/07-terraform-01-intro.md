# Домашняя работа к занятию "7.1. Инфраструктура как код"

Задание 1.
  
1. Какой тип инфраструктуры будем использовать для этого проекта: изменяемый или не изменяемый?

Если это возможно, то лучше использовать оба типа инфраструктуры: изменяемую, так как у нас нечеткое ТЗ, а неизменяемую для создания сред при разработке и перейти на неё, когда сервис уже будет стабильно работать .
2. Будет ли центральный сервер для управления инфраструктурой?

Так как в компании не исользуются такие инструменты, как Chef, Puppet и SaltStack, то наличие центрального сервера не требуется
3. Будут ли агенты на серверах?

Ansible, CloudFormation и Terraform, используемые в компании, не требуют установки дополнительных агентов
4. Будут ли использованы средства для управления конфигурацией или инициализации ресурсов? 

Будут использованы средства для управления конфигураций (Ansible) и инициализации ресурсов (terraform)

Какие инструменты из уже используемых вы хотели бы использовать для нового проекта? 

Packer для сборки образов, Docker для разворачивания контейнеров, Terraform для инициации ресурсов, Kubernetes для оркестрации, Ansible для управления конфигурацией на начальных этапах проекта.

Хотите ли рассмотреть возможность внедрения новых инструментов для этого проекта?

Возможно использование GitLab CI/CD для решения вопросов автоматизации


Задание 2. 
```
felimonist@feli:~$ terraform --version
Terraform v1.4.4
on linux_amd64
+ provider registry.terraform.io/yandex-cloud/yandex v0.88.0

Your version of Terraform is out of date! The latest version
is 1.4.6. You can update by downloading from https://www.terraform.io/downloads.html
```

Задание 3.

felimonist@feli:~# ln -s /usr/bin/terraform /usr/bin/terraform_v1.4.4

felimonist@feli:~# ln -s /home/felimonist/netology/07-terraform-01-intro /terraform /usr/bin/terraform_0.12

```
felimonist@feli:~$ terraform_v1.4.4 --version
Terraform v1.4.4
on linux_amd64
felimonist@feli:~$ terraform_0.12 --version
Terraform v0.12.0
```
