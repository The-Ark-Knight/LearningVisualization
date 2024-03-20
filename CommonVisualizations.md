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
