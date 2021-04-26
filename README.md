# Hledani-QR_kodu
`tracker.py` je program pro vyhledavani QR (i jiných) kódů v obrázku nebo video streamu.

Pro funkčnost je nutné mít nainstalováno:
* opencv (lze instalovat pomocí `pip opencv-python`)
* numpy
* pyzbar
* time

`tracker.py` obsahuje dvě hlavní metody s odlišnou funkcí
* `findallcodes(frame)` najde všechny kódy ve snímku, ohraničí je a vypíše nad ně jejich obsah
* `findcode(frame, data)` hledá pouze kódy obsahující řetězec předaný v parametru `data`, který ohraničí, vypíše obsah a nakreslí přímku od středu snímku ke středu kódu
