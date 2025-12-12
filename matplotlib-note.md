## Matplotlib 
Matplotlib is **a core Python library used for creating static, animated, and interactive data visualizations**. It provides a powerful, highly customizable interface for generating publication-quality plots across various platforms. 

1. **Install:** Open your terminal or command prompt and run:
    
    **bash**
    
    `pip install matplotlib`
    
2. **Import:** In your Python script or notebook, use the standard convention to import it:
    
    **python**
    
    `import matplotlib.pyplot as plt`
    

**Basic Plotting Example (Line Chart)**

The `pyplot` module simplifies the process of creating visualizations with a MATLAB-like syntax. Here is an example of creating a simple line chart:

**python**

```python
import matplotlib.pyplot as plt

*# Data for the plot*
x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]

*# Create the plot*
plt.plot(x, y)

*# Add labels and a title*
plt.xlabel("X-axis label")
plt.ylabel("Y-axis label")
plt.title("Simple Line Chart")

*# Display the plot*
plt.show()
```

**Common Plot Types**

Matplotlib can generate a wide array of plots:

- **Line charts:** `plt.plot(x, y)`
- **Bar charts:** `plt.bar(categories, values)`
- **Histograms:** `plt.hist(data, bins)`
- **Scatter plots:** `plt.scatter(x, y)`
- **Pie charts:** `plt.pie(values, labels)`

**Key Concepts**

- **Figure:** The entire window or page that contains all plots and elements.
- **Axes:** The actual area where the data is plotted, including the X and Y axes, ticks, and labels. A single Figure can contain multiple Axes (subplots).
