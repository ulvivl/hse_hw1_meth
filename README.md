# hse_hw1_meth
### №1

Отчеты Fastqc:<br>
Данные для SRR3414630_1 из второй домашки в первом семестре.

**Per base sequence content**

SRR5836475_1 | SRR3414630_1
--- | ---
![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/Per_b_sc_1.png) |  ![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/per_b_sq3.png)

Из особенностей можем наблюдать, что графики выглядят совершенно по-разному:<br>
Заметим, что в первом случае (SRR5836475_1) почти отсутствует Цитозин (C), по крайней мере его гораздо меньше чем в РНК, в отличие от Тимина (T) – его содержание, наоборот, больше, чем в РНК, cодержание Гуанина (G) и Ацетозин (А) же примерно на равном уровне, по сравнению с РНК (SRR3414630_1).<br>

**Per sequence GC content**

SRR5836475_1 | SRR3414630_1
--- | --- 
![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/Per_s_gc_1.png) |  ![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/Per_s_gc_3.png)

Видим, что на первом графике наблюдается нормальное распределение, однако немного смещенное.


### №2

[Colab с кодом](https://colab.research.google.com/drive/1QuP74Ola371aS37arV9O7BzrYBJgOFRI?usp=sharing)

**(a), (b)** Таблица с числм ридов, закартированных на участках 11347700-11367700; 40185800-40195800 и процентом дуплицированных прочтений для каждого образца

![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/table.png)

**(d)** M-bias plots<br>

Можем сказать, что на графиках изображен уровень метилирования для каждой возможной позиции в прочтении. На данных графиках по оси ```y``` слева видно значение Methylation calls, справа - пропорцию метилирования. Поскольку у нас парно-концевая запись, то для каждого запуска представлено 2 разных графика.

#### SRR3824222
Read 1 | Read 2 
--- | --- 
![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/Bismark_M-bias%20Read_1_22.png) | ![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/Bismark_M-bias%20Read_2_22.png) 
#### SRR5836475
Read 1 | Read 2 
--- | --- 
![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/Bismark_M-bias%20Read_1_75.png) | ![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/Bismark_M-bias%20Read_2_75.png)
#### SRR5836473
Read 1 | Read 2 
--- | --- 
![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/Bismark_M-bias%20Read_1_73.png) | ![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/Bismark_M-bias%20Read_2_73.png)

**(e)** Гистограммы распределения метилирования цитозинов по хромосоме (код находится в colab)

по оси X процент метилированных цитозинов, по оси Y - частота.
8cell | epiblast | icm 
--- | --- | ---
![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/8cell.png) | ![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/epiblast.png) |  ![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/icm.png)

Из графиков можно сделать вывод, что для каждого образца частота и процент метилированных цитозинов зависят по-разному. Для первого образца чаще всего метилируется 0%, почти в 40 процентов случаев. Для второго образца же, наоборот, чаще метилируется 100%, что достаточно хороший показатель, так как метилирование принимает участие в экспрессии гена. Ну и наконец третий образец, тут мы видим, что, чаще всего (почти в 60% случаев) метилируется 0% цитозинов.  

**(f)** Визуализация уровеня метилирования и покрытия для каждого образца.
Уровень метилирования | Уровень покрытия
--- | --- 
![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/met_level.png) | ![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/cov_level.png)
