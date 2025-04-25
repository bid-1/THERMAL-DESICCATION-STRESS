# THERMAL-DESICCATION-STRESS
Thermal profile vs Duration of aerial exposure
import matplotlib.pyplot as plt

# Data: Duration of aerial exposure (X-axis)
duration = [0, 2, 4, 6, 8]

# Data: Temperatures (Y-axis)
aerial_temperature = [25, 28, 30, 32, 34]  # Replace with your values
substratum_temperature = [22, 24, 25, 27, 28]  # Replace with your values
body_temperature = [36, 37, 38, 39, 40]  # Replace with your values

# Create the plot
plt.figure(figsize=(10, 6))
plt.plot(duration, aerial_temperature, marker='o', linestyle='-', color='red', label='Aerial Temperature')
plt.plot(duration, substratum_temperature, marker='s', linestyle='--', color='blue', label='Substratum Temperature')
plt.plot(duration, body_temperature, marker='^', linestyle='-.', color='green', label='Body Temperature')

# Add labels, title, legend, and grid
plt.title('Temperature Profiles vs Duration of Aerial Exposure')
plt.xlabel('Duration of Aerial Exposure (hours)')
plt.ylabel('Temperature (°C)')
plt.legend()
plt.grid(True)

# Show the plot
plt.show()
 # Plotting
>>> plt.figure(figsize=(10, 6))
<Figure size 1000x600 with 0 Axes>
>>>
>>> # Line plots with specific colors
>>> plt.plot(timestamps, aerial_temp, label='Aerial Temperature', marker='o', color='red')
[<matplotlib.lines.Line2D object at 0x0000023FBEDA9550>]
>>> plt.plot(timestamps, substratum_temp, label='Substratum Temperature', marker='s', color='blue')
[<matplotlib.lines.Line2D object at 0x0000023FC0A28310>]
>>> plt.plot(timestamps, body_temp, label='Body Temperature', marker='^', color='green')
[<matplotlib.lines.Line2D object at 0x0000023FC0A6CD50>]
>>>
>>> # Adding labels, title, and legend
>>> plt.xlabel('Duration of Aerial Exposure (hours)')
Text(0.5, 0, 'Duration of Aerial Exposure (hours)')
>>> plt.ylabel('Temperature (°C)')
Text(0, 0.5, 'Temperature (°C)')
>>> plt.title('Temperature Profiles during Tidal Emersion')
Text(0.5, 1.0, 'Temperature Profiles during Tidal Emersion')
>>> plt.xticks(ticks=timestamps, labels=duration)
([<matplotlib.axis.XTick object at 0x0000023FC0A3B550>, <matplotlib.axis.XTick object at 0x0000023FC0A39250>, <matplotlib.axis.XTick object at 0x0000023FBEAA6A50>, <matplotlib.axis.XTick object at 0x0000023FC0A6FED0>, <matplotlib.axis.XTick object at 0x0000023FC0A7A150>], [Text(0.0, 0, '0'), Text(1.0, 0, '2'), Text(2.0, 0, '4'), Text(3.0, 0, '6'), Text(4.0, 0, '8')])
>>> plt.legend(loc='upper right')  # Place the legend in the top-right corner
<matplotlib.legend.Legend object at 0x0000023FC0A283D0>
>>> plt.grid(False)  # Turn off the grid
>>>
>>> # Show the plot
>>> plt.show()
