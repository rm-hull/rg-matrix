# rg-matrix
A Raspberry Pi daemon to drive a 32x16 red/green LED matrix.

![Image of LED Matrix](images/s-l1600.jpg)

## Pinouts

| Board Pin | Name | Remarks                                            | RPi Pin | RPi Function |
|:---------:|------|----------------------------------------------------|:-------:|--------------|
| 1         | GND  | Ground                                             | 6       | GND          |
| 3         | GND  | Ground                                             | 6       | GND          |
| 5         | GND  | Ground                                             | 6       | GND          |
| 7         | OE   | 74HC595 Output Enable (Active Low)                 | tbc     |              |
| 9         | R    | data input for 74HC595 (RED section / 4*74HC595)   | tbc     |              |
| 11        | VCC  | +5V Power                                          | 2       | 5V0          |
| 13        | GND  | Ground                                             | 6       | GND          |
| 15        | GND  | Ground                                             | 6       | GND          |
| 2         | A    | row select wih 74HC138                             | tbc     |              |
| 4         | B    | row select wih 74HC138                             | tbc     |              |
| 6         | C    | row select wih 74HC138                             | tbc     |              |
| 8         | D    | row select wih 74HC138                             | tbc     |              |
| 10        | G    | data input for 74HC595 (GREEN section / 4*74HC595) | tbc     |              |
| 12        | VCC  | +5V Power                                          | 2       | 5V0          |
| 14        | STB  | 74HC595 Strobe / Data Latch                        | tbc     |              |
| 16        | SCK  | 74HC595 Clock Input                                | tbc     |              |

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
