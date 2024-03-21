# The following are a curation of the most common data visualization techniques we use and their respective implementation is python
Implementation is R will be added soon, though not a priority as of now.


### Scatter Plot: A scatter plot is used to visualize the relationship between two variables. It can be used to identify outliers, clusters, and trends in the data.

import matplotlib.pyplot as plt
import numpy as np
x = np.random.rand(50)
y = np.random.rand(50)
plt.scatter(x, y)
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.show()


### Line Plot: A line plot is used to visualize the change of a variable over time. It can be used to show trends and patterns in the data.

import matplotlib.pyplot as plt
import numpy as np

x = np.arange(0, 10, 0.1)
y = np.sin(x)

plt.plot(x, y)
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.show()


### Bar Chart: A bar chart is used to compare the values of different categories. It can be used to show the distribution of a variables

import matplotlib.pyplot as plt

categories = ['A', 'B', 'C', 'D']
values = [10, 20, 30, 40]
plt.bar(categories, values)
plt.xlabel('Categories')
plt.ylabel('Values')
plt.show()


### Histogram: A histogram is used to show the distribution of a variable. It can be used to identify the mean, median, and outliers in the data.

import matplotlib.pyplot as plt
import numpy as np

plt.hist(data, bins=30, alpha=0.6, color='g')

plt.xlabel('Value')
plt.ylabel('Frequency')
plt.title('Histogram of Random Data')

plt.show()


### Box Plot: A box plot is used to show the distribution of a variable and its quartiles. It can be used to identify outliers and compare the distribution of different groups.

import matplotlib.pyplot as plt

x = np.random.normal(size=1000)
y = np.random.normal(size=1000)

plt.boxplot([x, y])

plt.xlabel('Variable')
plt.ylabel('Value')
plt.title('Box Plot of Random Data')

plt.show()


### Heatmap: A heatmap is used to show the correlation between different variables in a dataset. It can be used to identify patterns and relationships in the data.

import matplotlib.pyplot as plt
import seaborn as sns

sns.heatmap(data, cmap='coolwarm')
plt.xlabel('Variable')
plt.ylabel('Variable')
plt.title('Heatmap of Random Data')

plt.show()


### Density Plot: A density plot is used to show the distribution of a continuous variable. It can be used to identify the mean, median, and the shape of the distribution.

import matplotlib.pyplot as plt
import numpy as np

plt.plot(x, np.full_like(x, 1 / len(x)), alpha=0.3)
plt.plot(x, np.full_like(x, 1 / len(x)), color='k')
plt.fill_between(x, np.zeros_like(x), np.full_like(x, 1 / len(x)), alpha=0.3)

plt.xlabel('Value')
plt.ylabel('Density')
plt.title('Density Plot of Random Data')

plt.show()