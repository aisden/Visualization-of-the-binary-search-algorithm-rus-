# Visualization-of-the-binary-search-algorithm-rus-
Описывает и реализует работу алгоритма бинарного поиска
Содержание
Введение	
Постановка задачи	
Часть 1. Описание алгоритма	
 1.1  Алгоритм бинарного поиска  с рекурсией	
1.2 Алгоритм  бинарного поиска без рекурсии итеративно	
Часть 2. Некоторые термины, программы, библиотеки и функции.	
2.1 Алгоритм бинарного поиска	
2.2 Libpng	
2.3 Apngasm 	
Часть 3. Некоторые термины, программы, библиотеки и функции.
3.3 Интерфейс программы 	
3.3.1 Интерфейс Visual Studio 	
3.3.2 Интерфейс apngasm	
3.3.3 Итог работы программы	
Заключение	
Список литературы	
Приложения	




			




 
Введение
Сегодня программирование является важной составляющей прогресса человечества. Миллионы людей напрямую или косвенно связаны с написанием кода, реализацией программ, выполнений алгоритмов. Последнее вообще тесно связано со всеми людьми – решение сложной задачи упрощается созданием системы последовательных методов и способов разрешения проблем. Язык, на котором написана моя курсовая – С, является очень старым. Но его разработка продолжается до сих пор. До сих пор многие программисты изучают этот язык. 
С - язык программирования общего назначения, который популярен из-за своей эффективности, экономичности и переносимости на другие программные платформы. Все эти преимущества обеспечивают качество разработки программного обеспечения, их быстроту и сравнительно небольшой размер. Программы, написанные на С по скорости работы можно даже сравнить с программами, написанными на языке ассемблер. 
Одним из примеров простого локального приложения может послужить созданная на языке C программа, реализующая алгоритм бинарного поиска в упорядоченном массиве
Стоит отметить и пояснить устройство и план курсовой работы.  Главе 1 приводятся основные этапы работы алгоритма бинарного поиска и излагается принцип поиска.  Глава 2 посвящена деталям проектирования приложения. Представлены примеры работы приложения и интерфейс взаимодействия с пользователем. В заключении приводятся результаты выполненной работы.
1.	Цель 
Написать программу, которая ищет индекс числа и демонстрирует непосредственно сам процесс.
2.	Исходные данные
Алгоритм бинарного поиска, литература по программированию
3.	Модель
Показ, визуализация алгоритма: поиск индекса числа в упорядоченном массиве
4.	Результат
Приложение, заливающее изображение и написанное на языке С, гиф-файл, показывающий процесс заполнения.
5.	Критерии оценки
•	Пользователь может выбирать вид бинарного поиска 
•	Пользователь может выбрать число элементов массива
•	анимированное изображение, показывающее процесс заливки
 
Часть 1. Описание алгоритма.
В процессе написания программы возникли трудности, которые оказались интересно решать.
1.1	Алгоритм бинарного поиска  с рекурсией
Программа получает число элементов массива и сам массив, заполненный случайными числами.  Затем программа Определяет значения элемента в середине структуры данных. Полученное значение сравнивается с ключом. Если ключ меньше значения середины, то поиск осуществляется в первой половине элементов, иначе  - во второй.
Поиск сводится к тому, что вновь определяется значение серединного элемента в выбранной половине и сравнивается с ключом.
Процесс продолжается до тех пор, пока не будет найден элемент со значением ключа или не станет пустым интервал для поиска.
После каждого пункта функция вызывает сама себя с измененными значениями 
1.2	Алгоритм  бинарного поиска без рекурсии итеративно.
Этот алгоритм почти ничем не отличается от алгоритма бинарного поиска с рекурсией. Лишь все действия программы вместо самовызова прописаны при помощи  циклов внутри функции. Пример этого кода можно посмотреть в приложении 

Часть 2. Некоторые термины, программы, библиотеки и функции.
2.1 Алгоритм бинарного поиска
 	Также известный как дихотомия, это  классический алгоритм поиска элемента в отсортированном массиве,  использующий дробление массива на половины. Используется в информатике, вычислительной математике и математическом программировании.

2.2 Libpng
Библиотека для работы с растровой графикой и которая написана на языке си называется libpng. Помимо вышесказанного, библиотека работает с изображениями формата .png. Для работы с приложением и непосредственно с программой и изображениями, была использована функция  png, рисовавшая пиксели на файле и сохраняющая их. 
Разобравшись с функциями рисования и записывания изображения, я перешёл к построению алгоритмов и разбору некоторых других необходимых для реализации работы частей.

 
2.3 Apng
Для создания анимации необходим инструмент apngasm — программа, объединяющая изображения формата png в одно целое с форматом apng. Данное приложение позволяет задать частоту смены кадров - можно отрегулировать анимацию под комфортную глазу скорость. Взаимодействовать с приложением можно, используя команды и функции командной строки.

 

Рисунок 1. Кадр работы с приложением apng.
 

Часть 3. Описание интерфейса программы и заливок блок схемы.
3.3 Интерфейс программы 
Ниже будут представлены кадры работы необходимых для курсовой приложений - Visual Studio и программа разработки анимированных изображений в формате apng. 
3.3.1 Интерфейс Visual Studio
 
Рисунок 2. Интерфейс программы.
Здесь представлен интерфейс программы с алгоритмом поиска  
На экран выводится отсортированный массив
 Выводится интерфейс выбора реализации алгоритма 
Далее выводится номер выбранного способа сортировки

 

3.3.2 Интерфейс apngasm
 
Рисунок 3. Меню apngasm
В данном меню (Рисунок 8) нас интересуют только первый и последний параметры. Первый устанавливает задержку между изображениями, последний устанавливает сколько раз повторится вся анимация. Ввод должен выглядит как: “apngasm64.exe output.apng  *.png 3”.
После этого будет создан файл output.apng, который можно открыть с помощью браузера.
3.3.3 Итог совместной работы и его демонстрация 
Для подведения промежуточного итога, было решено показать вам результат работы программы. В качестве объекта поиска выберем массив из 20 элементов, и находящееся в нем число 1. 
 
Рисунок 4. Испытуемый.

Далее будет процесс создания анимации, но, к сожалению, Microsoft Word не поддерживает динамические изображения и видео, поэтому файл будет отдельно от документа. И вы сможете его открыть, как уже было сказано, при помощи браузера.
 
Рисунок 5. Скриншот работы анимации. 
Заключение
Написание курсовой работы расширило диапазон знаний в области 
программировании  на языке Си. Приложение, которое было создано в рамках этого труда, сохраняет процесс поиска, который можно анимировать при помощи apng. 
Написание курсовой работы показало непонимание некоторого материала.
 		Например, работа со строковыми переменными. Было очень сложно изменять имя png файла согласно значению картинки (реализацию функции создания и сохранения точки можно посмотреть в приложениии). 
Были сложности с визуализацией  алгоритма сортировки. Продолжительный период времени, алгоритм отказывался компилировать имя файла согласно порядковому номеру создаваемой картинки.
 Касательно перспектив развития кода и этой курсовой работы, можно сделать визуализацию алгоритма бинарного поиска первого вхождения. 
 
Список литературы.
1.	[Электронный ресурс]. Режим доступа: свободный, 07.05.2020 19:27. Обзор и описание языка программирования С. Ссылка — http://unetway.com/blog/obzor-i-opisanie-azyka-programmirovania-si/
2.	Васильев Алексей, Программирование на С в примерах и задачах.  ООО “Издательство “Э”, 2017. - 592 с.
3.	[Электронный ресурс]. Режим доступа: свободный, 01.05.2020 11:52. Стек. Ссылка —https://prog-cpp.ru/data-stack/
4.	[Электронный ресурс]. Режим доступа: свободный, 30.04.2020 14:37. О стеке простыми словами — для студентов и просто начинающих. Ссылка — https://habr.com/ru/post/341586/
5.	[Электронный ресурс]. Режим доступа: свободный, 30.03.2020 19:35. libpng Home Page. Ссылка — http://www.libpng.org/pub/png/libpng.html
6.	[Электронный ресурс]. Режим доступа: свободный, 30.03.2020 21:38. A simple libpng example program. Ссылка — http://zarb.org/~gc/html/libpng.html
 
7.	Приложение
1. Фрагмент кода. Функция итеративного бинарного поиска с визуализацией.
static int BinarySearch_Iter(int array [], int key,int N, bitmap_t fruit, int c, char s[])
{
	//объявление переременных
	int left = 0;
	int right = N;
	int mid = 0;

	//пока границы не сошлись ввыполняй
	while (!(left >= right))
	{

		//поиск индекса  ср - эл та
		mid = left + (right - left) / 2;

		pixel_t * pixel = pixel_at(&fruit, left, array[left]);
		pixel->red = 0;
		pixel->green = 255;
		pixel->blue = 0;
		pixel->alpha = 255;
		//c++;
		c = png(0, 0, c, fruit, 0, s, 1);

		//закрашивание пикселя правой границы поиска
		pixel = pixel_at(&fruit, right, array[right]);
		pixel->red = 0;
		pixel->green = 0;
		pixel->blue = 255;
		pixel->alpha = 255;
		//c++;
		c = png(0, 0, c, fruit, 0, s, 1);

		//закрашивание пикселя среднего значения
		pixel = pixel_at(&fruit, mid, array[mid]);
		pixel->red = 255;
		pixel->green = 0;
		pixel->blue = 0;
		pixel->alpha = 255;
		//c++;
		c = png(0, 0, c, fruit, 0, s, 1);

		//если центральное значение раврняется ключу
		if (array[mid] == key)
		{
			//цикл закрашивания пикселей
			for (int i = 0 /*left*/; i <= N /*right*/; i++)
			{
				pixel = pixel_at(&fruit, i, array[i]);
				pixel->red = 255;
				pixel->green = 255;
				pixel->blue = 255;
				pixel->alpha = 255;
				//c++;
				c = png(0, 0, c, fruit, 0, s, 1);
				//условие незакрашивания ключа
				if (i == mid)
				{

					pixel = pixel_at(&fruit, i, array[i]);
					pixel->red = 255;
					pixel->green = 0;
					pixel->blue = 0;
					pixel->alpha = 255;
					//c++;
					c = png(0, 0, c, fruit, 0, s, 1);
				}
			}
			return mid;
		}
		//если элемент находится правее ключа
		if ((array[mid] > key) )
		{
			//закрашиваем правую границу после перестановки 
			for (int i = right; i > mid; i--)
			{
				//закрашивание пикселя
				pixel = pixel_at(&fruit, i, array[i]);
				pixel->red = 255;
				pixel->green = 255;
				pixel->blue = 255;
				pixel->alpha = 205;
				//c++;
				c = png(0, 0, c, fruit, 0, s, 1);
			}
			right = mid;
		}
		else
		{
			//закрашиваем левую границу после перестановки на место следующее за средним значением

			for (int i = left; i <= mid; i++)
			{
				pixel = pixel_at(&fruit, i, array[i]);
				pixel->red = 255;
				pixel->green = 255;
				pixel->blue = 255;
				pixel->alpha = 205;
				//c++;
				c = png(0, 0, c, fruit, 0, s, 1);
			}
			left = mid + 1;
		}
	}

	return (1 + left);
}
 
2.  Фрагмент кода. Функция создания точки и изменения имени файда. 
static  int png(int index, int n, int i,bitmap_t fruit,int arrayValue,char s[],int bool)
{
	// условие закрашивание пиксель в черный
	if (bool == 0)
	{
		// закрашивание пикселявчерный
		pixel_t * pixel = pixel_at(&fruit, index, arrayValue);
		pixel->red = 0;
		pixel->green = 0;
		pixel->blue = 0;
	}

	int a3;
	// запись изображения в файл'0000.png'.
	//объявляем переменные
	float f, dc1, dc2, cc1, cc2;
	f = i;
	//выделяем тысячную целую часть
	dc1 = modff((f-1)/1000, &cc1);
	dc2 = modff((f) / 1000, &cc2);

	if (cc1 < cc2)
	{
		s[0] = '0'+ cc2;
		s[1] = '0';
		s[2] = '0';
		s[3] = '0';
		if (cc2 > 0)
			f = f - cc2 * 1000;
	}
	else 
	{
		s[0] = '0' + cc1;
		if (cc1 > 0)
			f = f - cc1 * 1000;
	}
	
	dc1 = modff((f -1)/ 100, &cc1);
	dc2 = modff((f) / 100, &cc2);
	if (cc1 < cc2)
	{
		s[1] = '0'+cc2;
		s[2] = '0';
		s[3] = '0';
		if (cc2 > 0)
			f = f - cc2 * 100;
	}
	else
	{
		s[1] = '0' + cc1;
		if (cc1 > 0)
			f = f - cc1 * 100;
	}
	dc1 = modff((f-1) / 10, &cc1);
	dc2 = modff((f) / 10, &cc2);
	if (cc1 < cc2)
	{
		s[2] = '0' + cc2;
		s[3] = '0';
		if (cc2 > 0)
			f = f - cc2 * 10;
	}
	else
	{
		s[2] = '0' + cc1;
		if (cc1 > 0)
			f = f-cc1*10; 
	}
	dc1 = modff((f), &cc1);
	a3 = cc1;
	s[3] = '0' + a3;	
	save_png_to_file(&fruit, s);
	i++;
	return i;
}

