# java_demoqa_pageobjects_tests

Проект автоматизации тестирования UI для [DemoQA](https://demoqa.com) с использованием паттерна Page Object.

## Технологии

- Java 21
- JUnit 5
- Selenide
- Gradle

## Структура проекта
src/test/java/
├── pages
│ ├── TextBoxPage.java
│ └── components
│ ├── CalendarComponent.java
│ ├── ModalComponent.java
│ ├── StateCityComponent.java
│ └── TableComponent.java
├── tests
│ ├── TestStudentRegistrationForm.java
│ └── TextBoxTests.java
└── testdata
└── StudentRegistrationTestData.java
Особенности реализации
Реализован паттерн Page Object для разделения логики и тестов

Вынесены повторяющиеся элементы в компоненты (календарь, модальное окно, таблица)

Тестовые данные хранятся в отдельных классах

Поддержка позитивных и негативных сценариев

Результаты
✅ Регистрация студента (полная форма)

✅ Регистрация студента (только обязательные поля)

✅ Валидация обязательных полей (FirstName, LastName, Mobile, Gender)

