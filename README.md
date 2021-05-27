# Hledani-QR_kodu
`tracker.py` je program pro vyhledavani QR (i jiných) kódů v obrázku nebo video streamu.

Program byl testován na notebooku s Windows 10 s verzí pythonu 3.8.8.

Pro funkčnost je nutné mít nainstalované knihovny:
* opencv (lze instalovat pomocí `pip opencv-python`)
* numpy
* pyzbar
* time
ty lze nainstalovat i najednou pomocí requirements.txt příkazem `pip install -r requirements.txt` tím se nainstalují všechny potřebné knihovny pro tento program. V případě problémů s funkčností vyzkoušet více verzí opencv-python.

`tracker.py` obsahuje dvě hlavní metody s odlišnou funkcí
* `findallcodes(frame)` najde všechny kódy ve snímku, ohraničí je a vypíše nad ně jejich obsah
* `findcode(frame, data)` hledá pouze kódy obsahující řetězec předaný v parametru `data`, který ohraničí, vypíše obsah a nakreslí přímku od středu snímku ke středu kódu
