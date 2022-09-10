# taller3.histograma
"""
Created on Sat Sep 10 07:41:55 2022

@author: liseth
"""

from random import random
import matplotlib.pyplot as plt


#Datos aleatorios para el ejemplo
data1 = [int(random()*100) for _ in range(1000)]
data2 = [int(random()*10) for _ in range(200)]
data = [int(random()*10) for _ in range(200)]
data3 = [int(random()*90) for _ in range(500)]
data4 = [int(random()*200) for _ in range(3000)]
data5 = [int(random()*40) for _ in range(300)]


plt.title('datos aleatorios')
plt.hist(data1, bins=60, alpha=1, edgecolor = 'black',  linewidth=1)
plt.grid(True)
plt.show()
plt.clf()

fig, ax = plt.subplots(5, 2, sharey = True)
ax[0, 0].hist(data1, bins=60, alpha=1, edgecolor = 'black',  linewidth=1)
ax[1, 0].hist(data, bins=60, alpha=1, edgecolor = 'orange',  linewidth=1)
ax[2, 0].hist(data2, bins=60, alpha=1, edgecolor = 'red',  linewidth=1)
ax[3, 0].hist(data3, bins=60, alpha=1, edgecolor = 'green',  linewidth=1)
ax[4, 0].hist(data4, bins=60, alpha=1, edgecolor = 'blue',  linewidth=1)
ax[1, 1].hist(data5, bins=60, alpha=1, edgecolor = 'black',  linewidth=1)
ax[0, 1].hist(data, bins=60, alpha=1, edgecolor = 'red',  linewidth=1)
ax[2, 1].hist(data2, bins=60, alpha=1, edgecolor = 'green',  linewidth=1)
ax[3, 1].hist(data3, bins=60, alpha=1, edgecolor = 'orange',  linewidth=1)
ax[4, 1].hist(data4, bins=60, alpha=1, edgecolor = 'black',  linewidth=1)
