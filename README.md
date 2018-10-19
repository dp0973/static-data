# Static-data
A Python module for those tired of handling ddragon files to get champion/items names/images for League of Legends.

To install, run : 
```
pip3 install static-data
```

OR

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

For now, it only corresponds to my use cases, where I need to get name or image from champion or item having its name or id.

Feel free to ask for more.