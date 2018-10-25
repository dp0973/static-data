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

print(dd.getChampion("Annie").spell("Q").image)
print(dd.getChampion("Annie").spell(1).image)

print(dd.getSummoner("Flash").image)
#Change the patch to number 4, others settings (season and version) will be set at their last one)
dd.setVersion(patch=4)
print(dd.getSummoner("Flash").image)
```

For now, it only corresponds to my use cases, where I need to get name or image from champion or item having its name or id.

Feel free to ask for more.

Versions : 
 * 0.4.0 : 
     * Added runes reforged and fixed icons

 * 0.3.0 : 
     * Added champion spells and icons

 * 0.2.0 : 
 	 * Added summoners spells and maps
 	 * Fix the image url
 	 * Modified the version manager, instead of getLastPatch(), use getPatch(), without argument, to return the last patch Work for version and season as well.