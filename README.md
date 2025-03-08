## ФИО: Гук Егор Михайлович
## Преподаватель: Никита Карсканов

---

## Spring Boot Application

Аннотация `@SpringBootApplication` объединяет три ключевые аннотации Spring Boot:

- **`@SpringBootConfiguration`** – указывает, что класс является конфигурационным и может содержать определения бинов.
- **`@EnableAutoConfiguration`** – включает механизм автоматической конфигурации Spring Boot, который анализирует зависимости и настраивает приложение без необходимости явного определения бинов.
- **`@ComponentScan`** – активирует автоматическое сканирование компонентов (`@Component`, `@Service`, `@Repository`, `@Controller`) в текущем пакете и его подпакетах.

## Параметры аннотации `@SpringBootApplication`

| Параметр                 | Описание                                                                                                                                                      |
|--------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `exclude`                | Позволяет исключить определенные классы конфигурации из автоматической настройки. Принимает массив классов.                                                   |
| `excludeName`            | Исключает классы по их полным именам (в виде строки), что удобно при работе с динамическими конфигурациями.                                                   |
| `scanBasePackages`       | Определяет список пакетов, которые необходимо сканировать для поиска компонентов. Полезно, если бины находятся за пределами стандартного корневого пакета.    |
| `scanBasePackageClasses` | Позволяет задать классы, из пакетов которых Spring будет начинать сканирование компонентов. Используется, если нужно указать конкретные точки входа в пакеты. |
| `nameGenerator`          | Класс `BeanNameGenerator`, используемый для именования компонентов.                                                                                           |
| `proxyBeanMethods`       | Включает (`true`) или отключает (`false`) проксирование бином, что влияет на их создание и вызов методов внутри конфигурационного класса.                     |
# &#128521;