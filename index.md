# Python

Python (dále jen "Krajta") je programovací jazyk *rebelský* čili nerespektuje rodinu C-Like. Je tu tedy mnoho odlišností od "normálních" programovacích jazyků.

Jedná se o nejrychlejší jazyk co kdy byl vytvořen :)

## Komentář
Cokoli, co je napsáno za hashtagem (#) je ignorováno. Říká se tomu komentář

```py
# komentář

print(int(input("Číslo")) + 1) # toto je kouzlo
```

## Výpis textu nebo čísla
K výše uvedenému nám poslouží funkce `print`:

```py
print("Text") # uvozovky
print(3) # uvozovky nejsou nutné
```

Výstup
```
Text
3
```

Bohužel, Krajta je hloupý had, a za každý řádek vypisuje zalomení. Chceme-li spojit kousky dat, můžeme je vepsat do jediné funkce:

```py
print("Číslo", 3)
```

```
Číslo 3
```

## Proměnné
Proměnné se definují jako v matice.

```py
a = 3 # číslo
b = "Žluťoučký kůň úpěl ďábelské ódy." # text
nazevPromenne = "22" # taky text
x5hjyuhj2263_qwgqqw = 25 * 254 # nejlepší název proměnné. hodnota je výraz
```


### Výpis
Proměnné se do parametrů funkcí (takže i funkce `print`) předávají stejně jako v matice.

```py
a = 3
b = 5

print("a + b =", a + b)
```

### Vstup do proměnné
```py
a = input("Zadej textík")
b = int(input("A teď celé číslo"))
c = float(input("A teď jakékoli číslo"))
```

## Náhodná čísla
Sama krajta to neumí. Musíme ji obohatit o knihovnu vědění.

Nejlepší knihovna je `random` která je vestavěná, a přichází společně s instalací Krajty.

Knihovnu tedy importujeme.

```py
import random
```

A pak ji můžeme použít s funkcí `randint`.

```py
wernhvf = random.randint(2, 3)
```

Nebo lépe, nebudeme importovat celou knihovnu, jen tu potřebnou funkci. (Taky si nepůjčute domů celou knihovnu, ale jen pár knih.)
```py
from random import randint

ajicnh = randint(23123, 321546)


print(ajicnh) # Můžeme vypsat
```

## Podmínky

Kromě aritmetiky

```py
3 * 2
65 + 1
a / 2
aa ** 3
a - b
a ~/ 2123 # celočíselné dělení
```

Má krajta i logiku (avšak jako rebel nemá binární operátory)

```py
a = True and False == False # a nabývá hodnoty True
b = a and 2 < 3
c = a or b
```

## Větvení
```py
if 3 < 2:
	print("Fatal error")
else:
	print("Math just works")
```
Výstup záleží na tom, zda vás neozařuje kosmické záření.

### Mnohonásobné větvení
A roste stromeček! Krajta ale lézt neumí.

Zpátky k programování.

```py
k = int(input("Pick a number"))

if k < 65:
	print("Too low number")
elif k > 85452:
	print("Too high")
else:
	print("Too good number")
```

## Opakování
```py
for i in range(1, 10):
	for j in range(1, i):
		for k in range(2, 69):
			print("*", end=":")
	print()
```
