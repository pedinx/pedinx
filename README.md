import matplotlib.pyplot as plt
import numpy as np

# Dados
mexico = np.array([1.4, 2.5, 3.3, 4.3, 2.7, -6.0, -2.8, 0.4, 2.0, 2.9])
argentina = np.array([-2.5, 2.2, 8.0, 1.7, -10.0, -2.2, -1.5, 1.7, 1.9, 1.1])
brasil = np.array([3.2, 7.5, 2.8, 1.3, -0.6, -3.8, -2.3, 2.0, 3.2, 1.2])

# Figura
plt.figure(figsize=(12, 6))
plt.plot(mexico, label="México")
plt.plot(argentina, label="Argentina")
plt.plot(brasil, label="Brasil")
plt.xlabel("Ano")
plt.ylabel("Crescimento anual do PIB (%)")
plt.legend()

# Salvar a figura
plt.savefig("crescimento-pib.png")
