```python
import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv("sample-data.csv")

#convert timestamp
df['timestamp'] = pd.to_datetime(df['timestamp'], errors='coerce')

#drop missing timestamps
df = df.dropna(subset=['timestamp'])

plt.plot(df['timestamp'], df['bytes'])
plt.xlabel("Time")
plt.ylabel("Bytes")
plt.title("Bytes Over Time")
plt.xticks(rotation=45)
plt.tight_layout()
plt.show()

```

<img width="640" height="480" alt="Figure_1" src="https://github.com/user-attachments/assets/d27936b1-51b8-40f3-8a58-ebcee257697e" />
