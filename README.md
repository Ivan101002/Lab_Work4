# Виртуальная и дополненая реальность
Отчет по лабораторной работе #4 выполнил
- Попович Иван Алексеевич
- РИ-300022
Отметка о выполнении заданий (заполняется студентом):

| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | * | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- 
- 
- 


Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 2.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 3.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.
- ✨Magic ✨

## Цель работы
Изучить принципы создания и настройки передвиженияпользователя в VR с помощью стиков на контроллерах и с помощью телепортации.

### Пошагово выполнить каждый пункт по примеру предоставленных видеоматериалов:
- Открыть проект из 3 лабораторной работы;
- Зайти в Unity Asset Store, выбрать подходящие ассеты и импортироватьих в проект;
- Создать новый материал. Выбрать текстуру будущего пола среди скачанных ассетов. Добавить созданному материалу выбранную текстуру;
- Изменить у материала значения параметров Tiling на подходящие;
- Созданный материал добавить на Plane;
- Выбрать модель стен из префабов среди скачанных ассетов;
- Разместить несколько стен в ряд;
- Скопировать ряд стен и разместить на каждую сторону;
- Разделить большую комнату на две маленькие с помощью скопированных стен;
- Удалить среднюю стену у перегородки;
- Скопировать пол, перевернуть и вставить в качестве потолка;
- Добавить модели факелов на стены;
- Расставить освещение;
- В первую и вторую комнату по центру поставить префаб стола из скачанных ассетов;
- Создать объект (камень);
- Добавить на него Collider и Rigidbody;
- Добавить на объект GrabInteractible;
- Добавить на контроллеры XR Direct Interactor;
- Добавить Outline;
- Написать скрипт, управляющий включением подсветки;
- Запустить проект и проверить работоспособность;
- Включить физику в Rigidbody на объекте;
- Включить Throw on Detach на GrabInteractible;
- Запустить проект и проверить работоспособность;
- Создать Ray Interactor;
- Настроить внешний вид луча;
- Установить Interaction Layer Mask, чтобы не телепортироваться лучом;
- Продемонстрировать притягивание;
- Написать скрипт для управления появлением/исчезанием луча;
- Запустить проект и проверить работоспособность.


Скриншот сцены в Unty 3d после выполнения всех указаных действий в задании №1
![](/L4.png)



## Задание 2
### Какой компонент позволяет добавить взаимодействие с объектами в VR? Привести развернутый ответ с примерами.
Ответ:
XRDirectInteractor - применяется для взаимодействия с различными интерактивными объектами для соприкасновения. Он обрабатывается с помощью триггеров, которые обновляют текущие допустимые объекты для данного интерактора. Данный объект должен иметь объем столкновения для срабатывания триггеров. 
SphereCollider - позволяет идентифицировать, что мы дотронулись до объекта
XRGrabInteractable - позволит нам взаимодействовать с объектом внутри виртуальной реальности

Пример: Если нам нужно взять шар, но нужно учесть радиус в SphereCollider, иначе объект будет отлетать.


# Задание 3
### В чём разница между Velocity tracking, Kinematic и Instantaneous Movement Type? Привести развернутый ответ с примерами.

Ответ:
Kinematic - Используется когда необходимо чтобы объект с которым мы взаимодействуем перемещался через другие коллайдеры, не застревая вслед за нашими руками.

Пример: Если нужно проверять триггер на объете без физики, то выбираем тип Kinematic.

Velocity tracking - Движется мнговенно за нашим интерактором(руки), перемещается через другие коллайдеры без Rigidbody, движения болле резкие.

Пример: Используется для того чтобы адекватно реагировать на коллайдеры и не трясти объект

Instantaneous Movement - Плавный, но он не перемещается через другие Rigidbody коллайдеры, снижает задержки и делает движение более естественными.

Пример: Если движения должны быть плавными, природными, натуральными

## Выводы

Во время выполнения этой работы, я дополнил предыдущую лаб. работу и научился новым фишкам в 

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**

