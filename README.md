# hse_hw1_meth
### №1

Отчеты Fastqc:




### №2

[Colab с кодом](https://colab.research.google.com/drive/1QuP74Ola371aS37arV9O7BzrYBJgOFRI?usp=sharing)

**(a), (b)** Таблица с числм ридов, закартированных на участках 11347700-11367700; 40185800-40195800 и процентом дуплицированных прочтений для каждого образца

![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/table.png)

**(d)** M-bias plots<br>

Можем сказать, что на графиках изображена пропорцию метилирования для каждой возможной позиции в прочтении. На данных графиках по оси ```y``` слева видно значение Methylation calls, справа$~-~$пропорцию метилирования. Поскольку у нас парно-концевая запись, то для каждого запуска, представлено 2 разных графика.

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

Из графиков можно сделать вывод, что для каждого образца частота и процент метилированных цитозинов зависят по-разному. Для первого образца наиболее часто метилируется 0%, почти в 40 процентов случаев. Для второго образца же, наоборот, наиболее часто метилируется 100%, что достаточно хороший показатель, так как метилирование принимает участие в экспрессии гена. Ну и наконец третий образец, тут мы видим, что, чаще всего (почти в 60: случаев) метилируется 0% цитозинов.  

**(f)** Визуализация уровеня метилирования и покрытия для каждого образца.
Уровень метилирования | Уровень покрытия
--- | --- 
![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/met_level.png) | ![](https://github.com/ulvivl/hse_hw1_meth/blob/main/img/cov_level.png)
