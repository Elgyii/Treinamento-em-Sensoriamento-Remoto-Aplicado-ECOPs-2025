# Semana 1 – Actividades Práticas

## Dia 1 – Criação do Ambiente

### Mínimo obrigatório ✅

- [ ] Criar ambiente Python (Conda/Colab)
- [ ] Instalar bibliotecas básicas (`numpy`, `pandas`, `xarray`, `matplotlib`, etc.)
- [ ] Inicializar o ambiente e faz o `import` das bibliotecas

```python
# Exemplo de import
import numpy as np
import pandas as pd
import xarray as xr
import matplotlib.pyplot as plt

# Teste simples
print("Versões instaladas:")
print("numpy:", np.__version__)
```

Opcional

- Explique passo a passo, os problemas enfrentados e soluções implementadas

## Dia 2 – Visualização de Dados

### Mínimo obrigatório ✅

- [ ] Criar uma imagem em matplotlib (clorofila ou SST)
- [ ] Adicionar título e legenda

```python
# Exemplo mínimo de visualização (dados fictícios)
import numpy as np
import matplotlib.pyplot as plt

# simula CHL ou SST
data = np.random.rand(50, 50)
plt.imshow(data, cmap='viridis')
plt.colorbar(label='CHL [mg/m^3]')
plt.title("Exemplo de Clorofila")
plt.show()
```

---

### Questões Opcionais

- [ ] Criar as duas imagens (CHL + SST)
- [ ] Adicionar mapa geográfico (cartopy)
- [ ] Fazer uma breve interpretação científica

```python
# Exemplo basico
import cartopy.crs as ccrs
import cartopy.feature as cfeature

fig = plt.figure(figsize=(6,4))
ax = plt.axes(projection=ccrs.PlateCarree())
ax.coastlines()
ax.add_feature(cfeature.LAND)
ax.add_feature(cfeature.OCEAN)
plt.title("Mapa Geográfico")
plt.show()
```

---

### Notas Finais

- O que foi simples de entender e executar?
- Onde enfrentou mais dificuldades e quais foram?
- Conseguiu resolver as dificuldades forma individual? Como?

- Crie um ambiente Python funcional (Conda/Colab)
- Instale as bibliotecas básicas (numpy, pandas, xarray, matplotlib, etc.)
- Inicialize o ambiente e faz o `import` das bibliotecas
- `Opcional:` Explique passo a passo, os problemas enfrentados e as resoluçoes adoptadas.

---

### Dia 2 (Visualização de Dados)

Escolha uma área de interesse e faz:

- Crie uma imagem de clorofila ou SST (mínimo obrigatório)
- Adicione legendas e titulos

`Opcional 1:` Crie as duas imagens <br> `Opcional 2:` Adicione o mapa geográfico (cartopy) <br> `Opcional 3:` Faça uma
breve interpretação científica
