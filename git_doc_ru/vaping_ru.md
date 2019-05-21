### Меню парения ( Vaping )
 
 ![Vaping menu](https://i.imgur.com/w7wkvhg.png) ![Vaping menu](https://i.imgur.com/CeAKp9k.png)

* __Preheat ( предварительный нагрев )__
    
	![preheat menu](https://i.imgur.com/MCSGVT4.png)
        
    *Может работать в режимах вариватта ( POWER ) и смарта ( SMART ), в других игнорируется.*  
    
    *Этот пункт меню так же показывается по кликам на кнопку Пуск, если на эти клики выбрано действие (**PPwr**) - приоритет мощности.*
    
    Используется для разогрева тяжелых холодных намоток.  
    Если включен преднагрев, то на основном экране режима POWER у показателя мощности появится значок "**p**".

    - Enable - Включить / выключить преднагрев.

    - Возможно установить мощность ( Pwr ) и время ( Time ). На это время будет подаваться указанная мощность при затяжке.  
    После этого будет подаваться основная мощность.
        
    - Unit - менять мощность преднагрева в Ваттах или процентах от основной.   

    - Delay - время задержки для следующего преднагрева, до 3-х минут. Пока тикает это время, прехит не включается и значёк "p" мигает.  
    (это время является общим и для меню Кривых парения)
    
    - SMART - умный преднагрев, два режима:  
    	- Режим увеличения времени.  
    Для примера работы установите время преднагрева (Time) 1 сек и задержку до следующего включения преднагрева (Delay) 10 сек.  
    Первая затяжка пойдёт с установками обычного преднагрева. Далее, если вторая затяжка началась через 5 секунд (половина от установленного времени задержки), то время преднагрева будет 0.5 сек (так же половина). И так далее в процентном соотношении, чаще затяжки - меньше врема преднагрева и наоборот.  
    (взято по описанию для прошивки Vortex Mod).  
    
    	- Режим нарастания мощности.  
			Пока истекает время задержки, мощность преднагрева для  следующей затяжки растет от выставленной основной мощности до установленной мощности преднагрева. Чаще затяжки - меньше мощность преднагрева и наоборот.   
            
		Пока идет время умного преднагрева, рядом с мощностью мигает знак "**s**".
  

* __Curve ( Кривые нагрева )__

	![curve menu](https://i.imgur.com/WV9MVY1.png) ![curve menu](https://i.imgur.com/aiOh12o.png)

    *Может работать в режимах вариватт ( POWER ) и смарт ( SMART ), в других игнорируется.*  
    
    Имеет приоритет ниже, чем у преднагрева.  
    Включенное состояние показывается значком "**c**" рядом с мощностью. Значок мигает во время задержки перед новым использованием (Delay).
    Каждый профиль может иметь одну настроенную кривую нагрева.
  
    - Enable: включить / выключить использование кривой.
    - Reset: сброс кривой. Сделайте это до первого редактирования. Мощность на всем протяжении установится на 100% ( текущая выставленная ). Для ресета долго удерживайте кнопку фаер.
    - Edit: окно редактирования кривой.  
            Кнопками (+-) выбрать время, нажать Пуск, кнопками выбрать мощность, которая будет установлена после этого времени во время затяжки.  
            Мощность меняется 0 - 200% от основной. 20 точек регулировки, максимальная длительность кривой - 5 секунд.
    - Delay: время задержки перед повторным использованием данной функции.
    - Repeat: время, после которого кривая нагрева зацикливается сначала, до времени отсечки парения.

* __Algo ( Алгоритмы ТК )__

	*Только для режимов термоконтроля.*  

	![Algo submenu](https://i.imgur.com/CS7o6oU.png)  

    Несколько алгоритмов на выбор, переключение по кнопке Пуск:
    - Off: выключено, используется алгоритм из официальной прошивки.
    - Sweet: более легкий старт.
    - Boost: резкий старт, с регулировкой.
    - PID: Пропорционально-интегрально-дифференцирующий (ПИД) регулятор с редактированием всех параметров.
         
    Лучший алгоритм, но требует настройки, настраивайте и проверяйте, программа-монитор в помощь.  

    - Boost - регулировка для алгоритма быстрого старта.  
            Устанавливает предел температуры в процентах от основной, после достижения которой прекратится резкий нагрев.  
            Чем больше значение, тем быстрее разогрев до заданной температуры, но есть риск выхода за пределы установки. уменьшите максимум мощности ТК, чтобы это предотвратить.  
            Стоит устанавливать выше для тяжелых намоток и меньше для простых.

* __P, I, D ( регулировка ПИД )__
      
    Долгое нажатие Пуск вернет настройки каждого пункта в исходное.  
    - P - пропорциональная часть (Proportional), по умолчанию 600. Чем выше, тем быстрее разогрев.  
    - I - интегральная часть (Integral), 850. Чем выше, тем более плавное поддержание.  
    - D - дифференциальная часть (Derivative), 0. Повышает быстродействие выхода на заданную температуру.  

    Как это работает - расскажет гугл.  
    Значения по умолчанию служат, чтобы подходить большинству пользователей, но для частных случаев требуется корректировка.  
    Единицы измерения: **P** mW/°C, **I** mW/°C/s, **D** mW.s/°C.

* __Modes ( Пропуск режимов )__

	![modes](https://i.imgur.com/aVi3SSn.png)

    Если напротив режима стоит (**N**) - данный режим не показывается при прокрутке режимов на главном экране.  
    Например можно отключить показ режима Байпас в много-батарейных модах. А кому то не нужен Смарт.  
    Активный режим (**A**) нельзя исключить (должен быть хотя бы один).  

* __Prot. ( Отсечка затяжки )__

    Установка максимального времени затяжки, после которого она прекращается с предупреждением.  
    Если продолжать удерживать кнопку Пуск - мод выключится, думая, что это случайное нажатие, например в сумке.  
    А вообще всегда выключайте мод кликами. По умолчанию 3 или 5 кликов.
    Регулировка от 2 до 25 секунд, по умолчанию 10. Лучше настройте под ваш стиль.
        
* __Vaped ( Выпаренное )__ 

	Для приблизительного подсчета выпаренного в миллилитрах требуется подстроить коэффициент **ml/kJ**. Это можно сделать в этом окне кнопками ( +- )  
    По умолчанию, соответствует парению около 30-ти Ватт.  
    Для сигаретной тяги хороший результат был при коэффициенте 300.  
    **Настройка:** Залейте в бак извествое количество жижи, обнулите счетчик общего выпаренного, выпариваете жижу, и в этой настройке крутите коэффициент, пока число выпаренного не станет таким же.
    
	На экране так же показаны текущие значения:  
    - выпарено всего, в мл
    - выпарено за день, в мл
    - затраченная энергия, в Ватт-час
    - время парения
    - количество затяжек
    
    ![mlkj](https://i.imgur.com/CTlXCdb.png)

* __PuffOff ( выключение по затяжкам )__

    Выбор количества затяжек перед выключением мода. Регулируйте свои перепары, чтобы не получить передоз. Хорошее значение - 13, примерное количество тяг сигареты (которые мы бросили, перейдя на пар).  
    Off - выключение работы функции.

* __TmrOff ( выключение по времени работы )__

    Установка времени работы мода перед его автоматическим выключением. Считается всё время работы, пока мод не уснул.  
    Off - выключение работы функции.  
    
    *Нажатие кнопки плюс на выключенном моде покажет почему мод был автоматически выключен (по затяжкам, по времени работы, по защите от долгого нажатия кнопки Пуск...).*
    
* __HoldFi ( запрет парения )__

    Установка в минутах до одного часа времени запрета парения после выключения мода по достижении заданного количества тяг (**PuffOff**) или по времени работы (**TmrOff**).  
    Off - выключение работы функции.  
    Во время запрета парения в верхней строке будет отображаться оставшееся время запрета и почему мод был до этого автоматически выключен (T - по времени, P - по затяжкам). При этом регулировка этого времени в меню запрещена и парить мод не даст - перепар закончен, отложите мод и это Ваш выбор.  
    Эта функция автоматически включает режим лёгкого сна (LSL), потребление вырастет. ***Поэтому выключайте этот режим, если долго не будете заряжать мод, особенно со встроенными батареями!***  
   
* __VVLite ( легкий варивольт )__

    При включении этой функции мод превращается в варивольт.  
    Отдельного окна для режима нет ( поэтому легкий ), все делается в режиме мощности ( POWER ). Иконка напряжения на основном экране изменится.  
    Как обычно, выставляете мощность для парения, этим вы меняете и **напряжение, которое в процессе затяжки меняться уже не будет**.  
    Для достижения точности установки напряжения - включите режим изменения мощности по 0.1 Ватту в меню Интерфейса.
    
* __AutoFi ( Автофаер )__

    Режим автоматического "огня", без удерживания кнопки Пуск все время.  
    **Запуск** - чуть дольше нажать на кнопку Пуск, затем отпустить. Мод продолжит подавать мощность заданное в пункте (**ATime**) время.  
    Повторный клик на Пуск отменит затяжку.  
    Off - выключение работы функции.

* __ATime ( время автофаера )__

    Настройка времени для автоматического парения (**AutoFi**).  
Можно выставить **бесконечную** подачу мощности ( значок бесконечности, для самодельных фонариков, паяльников или тестирования )

* __Repeat ( повтор, реплей )__

    Заменяет режим термоконтроля на более простой в вариватте.  
**Только для спиралей из материалов для термоконтроля.**  

	![replay](https://i.imgur.com/Yvy7K38.png) ![replay](https://i.imgur.com/BsjYtVr.png) ![replay](https://i.imgur.com/PEmk5uA.png)  
    
	- установив эту галочку, переходим в режим POWER и, подбирая мощность, делаете затяжки, пока Вас не устроит результат.  
    - последнее сопротивление нагретой спирали и выставленная мощность сохраняются.  
 	- что бы повторить эту затяжку (реплей), нужно **заблокировать** кнопки (+-), удерживая их.
 	-  при следующих затяжках запомненное сопротивление нагретого койла будет поддерживаться постоянным ( как температура в режимах термоконтроля ).  

	Для индикации режима справа от числа мощности будет гореть буква "**r**". Если материал спирали не подходит, парение в режиме повтора может быть остановлено и режим выключен автоматически.

* __PwrLo ( понижение мощности )__
	Если включено, то мод будет автоматически понижать установленную мощность, если заряда батарей для этого не хватает.

-----

← Предыдущая страница: [Меню спиралей](coils_ru.md) --  Следующая страница: [Меню часы ](clock_ru.md)→