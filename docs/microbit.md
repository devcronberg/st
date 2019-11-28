# BBC micro:bit

![](https://microbit.org/images/microbit-hardware-access.jpg)

## Bag micro:bit

- "The Micro:bit Educational Foundation"
  - Fra 2015
  - None profit
  - "Our vision is to inspire every child to create their best digital future"
  - Stiftere/bidragsgivere
    - BBC
    - ARM
    - Microsoft
    - Amazon
    - British Counsil
- Se [https://microbit.org](https://microbit.org)
- BBC micro:bit har rødder tilbage til [BBC Micro](https://en.wikipedia.org/wiki/BBC_Micro) fra 80'erne 

## Hvad er en BBC micro:bit

- Lille simpel microcontroller baseret på en 16 MHz 32bit ARM Cortex-M0 processor med 256 KB Flash og 16 KB RAM. Alt hardware er open source.
  - 25 LED
  - To knapper
  - Accelerometer (acceleration)
  - Magnetometer (kompas)
  - Temperaturføler
  - Lysføler
  - Bluetooth / Radio
  - USB
  - 25 I/O porte til forskellige sensorer, motorer, lamper mv
    
## Programmering

![](https://microbit.org/images/both-editors.png)

- Kan programmeres på mange måde men typisk bruges enten 
  - [MakeCode (eller JavaScript)](https://makecode.microbit.org/) - link til online MS MakeCode Editor (dansk)
  - [Python](https://python.microbit.org/v/2.0) - link til online Python editor
- Men der findes [mange andre muligheder](https://en.wikipedia.org/wiki/Micro_Bit#Software) - herunder C++, Rust, MatLab, BASIC, Assembler og mange flere

### Eksempel på MakeCode

![](makecode.png)

### Eksempel på JavaScript

```
input.onButtonPressed(Button.A, function () {
    basic.showString("" + input.compassHeading())
})
input.onButtonPressed(Button.B, function () {
    basic.showString("" + input.lightLevel())
})
```


### Eksempel på Python

```
import microbit

while True:
    if microbit.button_a.is_pressed() and microbit.button_b.is_pressed():        
        microbit.display.scroll("")
    elif microbit.button_a.is_pressed():
        microbit.display.scroll(microbit.compassHeading())
    elif microbit.button_b.is_pressed():
        microbit.display.scroll(microbit.lightLevel())
    microbit.sleep(100)
```

## Dokumentation

- Der findes masser af dokumentation 
  - [https://microbit.org/guide/quick/](https://microbit.org/guide/quick/) - engelsk (og andre sprog)
  - [https://www.dr.dk/skole/ultrabit](https://www.dr.dk/skole/ultrabit) - dansk

