### __Меню cпиралей ( Coils )__
   ![coils](https://i.imgur.com/zk9yxSI.png)
* __Manage ( Коррекция сопротивлений )__ 
  
  ![coils](https://i.imgur.com/1LvyceE.png)  
  
  Четыре строки для каждого вида термоконтроля:  
  При входе в это меню будет выбрана строка для текущего режима термоконтроля (если таковой выбран).  
  Выбрав нужную строку, кликнуть Пуск для входа в режим редактирования сопротивления.  
  Скорректировать сопротивление кнопками ( + - ).  
  Нажатие на Пуск без редактирования изменит состояние блокировки койла (замок).  
  Редактирование не нулевого сопротивления автоматически заблокирует его.  
  Долгое нажатие на Пуск перечитает сопротивление койла заново.  
 
 
* __Zero All ( Обнуление )__
  Очистка всех запомненных модом сопротивлений, включая режимы Смарт и Вариватт.  
* __TCR ( Предустановки термоконтроля )__

  ![tcr](https://i.imgur.com/b0POA6N.png)  
        
   В дополнение к трём настраиваемым режимам ТК (M1, M2, M3) можно установить фиксированные значения для остальных режимов ( TEMP NI, TI, SS ). Для этого:
   * Выбрать режим для разблокировки,
   * Долгим нажатием кнопки Пуск разлочить данный пункт. Подходящее значение появится на экране, его можно редактировать.
   * Повторное долгое нажатие Пуск вернёт настройку по умолчанию (DEF).  

	( PW ) Чтобы показывать температуру койла в режимах вариватта, нужно выбрать алгоритм вычисления из имеющихся, выберите материал Вашего койла или его предустановленный ТКС (температурный коэффициент сопротивления).
 
* __Profile ( Профили )__ >> [Меню профилей](profiles_ru.md)

* __Smart ( авто-профиль )__
  Автоматический выбор профиля для установленного атомайзера. Границы сопротивления устанавливаются в процентах в настройке "New".
  Сначала требуется настроить профиль и сохранить.  
  Отключите эту возможность, если мод не может четко замерить сопротивление ("плавает").
  
* __Cold ( Базовая температура )__
  По умолчанию 20 градусов Цельсия. Мод считает, что эта минимальная температура, при которой пользователь блокирует сопротивление для ТК. Это значение участвует в результате расчета температуры спирали как простая добавка.
  

* __New ( Новый койл? )__
  Если сопротивление в ТК не заблокировано, мод может определить, что установлен другой бак, если его сопротивление отличается на этот заданный процент. По умолчанию 5%.
  
  
* __Check: Yes/No ( Проверка совместимости )__
  Мод проверяет спираль на возможность работы с термоконтролем. "Тяжелые" койлы могут не пройти проверку на ТК (мод переключится в режим вариватта), хотя могут работать и в этом режиме. Данная галочка может отменить эту проверку (No).  

-----

← Предыдущая страница: [Меню экрана](screen_ru.md) --  Следующая страница: [Меню парения ](vaping_ru.md)→