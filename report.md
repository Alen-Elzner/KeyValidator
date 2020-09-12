## Краткое описание

10.09.2020 - 10.09.2020 было проведено тестирование установки, функциональное тестирование, дымовое тестирование приложения KeyValidator.

### На тестирование затрачено: 15мин

### В результате тестирования выявлены следующие дефекты:

* [Валидный ключ считается невалидным](https://github.com/Alen-Elzner/KeyValidator/issues/1)
* [НЕвалидный ключ считается валидным](https://github.com/Alen-Elzner/KeyValidator/issues/3)

## Описание процесса тестирования

### В процессе тестирования использовались следующие артефакты:

1. [Описание задания](https://github.com/netology-code/javaqa-homeworks/tree/master/intro)

1. [Инструкция по установке OpenJDK11](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md)

1. [Руководство использования](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md)


### В качестве тестовых данных использовались данные из Руководство использования:

**Валидные ключи**:

* 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998
* 80b427f8-92cd-3aae-ba04-3927fbe17c6
* b295bc63-9f03-3b4b-af80-969b39f8c262
* 387eedc6-12e9-3b32-9881-63b6b5e85317
* c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180

**Невалидные ключи**:

* 18252235-78e0-44a5-8720-556f0c7da17a
* e66075b6-ddad-445e-baf6-161b3289522b
* b6d53250-f07e-4352-a293-6102ddf7f1ca
* c2bc778a-1cb9-46c6-b435-0489649d2a42
* 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1

В результате работы вывод приложения будет выглядеть следующим образом:
```
Result for 00000000-0000-0000-0000-000000000000: OK
Result for 00000000-0000-0000-0000-000000000001: FAIL
```
где **OK** означает, что ключ валидный, **FAIL** - невалидный.

### Тестирование производилось в следующем окружении:

* Windows 8.1 професиональная build 9600
* openjdk version "11.0.8" 2020-07-14
* OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.8+10)
* OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.8+10, mixed mode)
