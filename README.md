# Static-data
A Python module for those tired of handling ddragon files to get champion/items names/images for League of Legends.

Download and run 
```
python setup.py install
```

Use : 

```python
from static_data import ddragon
dd = ddragon.ddragon()
print(dd.getChampion("Annie").image)
print(dd.getChampion(1).image)
print(dd.getChampion(1).name)
```
