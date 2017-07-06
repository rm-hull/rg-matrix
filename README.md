# rg-matrix
A Raspberry Pi daemon to drive a 32x16 red/green LED matrix.

![Image of LED Matrix](images/s-l1600.jpg)

## Pinouts

| Desc | Pin | Pin | Desc |
|-----:|:---:|:---:|------|
|  GND |  1  |  2  | A    |
|  GND |  3  |  4  | B    |
|  GND |  5  |  6  | C    |
|   OE |  7  |  8  | D    |
|    R |  9  |  10 | G    |
|  VCC |  11 |  12 | VCC  |
|  GND |  13 |  14 | STB  |
|  GND |  15 |  16 | SCK  |

* __A, B, C, D__ - row select with 74HC138
* __OE__ - 74HC595 Ouput Enable(Active Low)
* __STB__ - 74HC595 Strobe / Data Latch
* __SCK__ - 74HC595 Clock Input
* __R__ - data input for 74HC595 (RED section / 4*74HC595)
* __G__ - data input for 74HC595 (GREEN section / 4*74HC595)

## References

* http://www.ebay.co.uk/itm/351368537705
* http://www.embeddedadventures.com/datasheets/LDP-6416.pdf
* http://www.instructables.com/id/32x16-LED-Matrix-Panel-and-Arduino/

## License

### MIT License

Copyright (c) 2017 Richard Hull

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
