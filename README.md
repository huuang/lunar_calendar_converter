## Using

Import the library:

```dart
import 'lunar_solar_converter.dart';
```

<br>

You can use this converter to convert calendar from one to another between lunar calendar and solar calendar. 
For example:
  ```
Lunar lunar = Lunar(lunarYear: 2022, lunarMonth: 4, lunarDay: 1, isLeap: true);
Solar solar = LunarSolarConverter.lunarToSolar(lunar);
   ```
   
  or
  
  ```
Solar solar = Solar(solarYear: 2018, solarMonth: 8, solarDay: 22);
Lunar lunar = LunarSolarConverter.solarToLunar(solar);
   ```
<br>

  The `Lunar` class can also come out Chinese text for a lunar calendar, such as:
  ```
  Lunar lunar = Lunar(lunarYear: 2018, lunarMonth: 8, lunarDay: 22);
  print(lunar);
   ```
  
  You will get `庚子年(2020)闰四月初一`.