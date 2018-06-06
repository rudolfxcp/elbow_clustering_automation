# elbow_clustering_automation
Данная задача решалась для одномерного случая (кластеризация 2000 групп товаров по весу). 
В данном примере рассматривается только случай со сгенерироваными значениями.

Для определения оптимального количества кластеров использовался метод локтя (elbow method). Но поскольку он графический, то
возникла необходимость автоматизировать нахождение оптимального количества кластеров.

За основу определения наилучшего количества кластеров была взята площадь под кривой. 
Перед этим данные прошли определенную стандартизацию. 
За основу работы использовался схожий метод определения наилучшего порога в ROC_AUC. 

Не работает (но легко допиливается) для случаев:
- если только одно значение
- если значений меньше 20
- если все значения равны 
