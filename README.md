# rg-matrix
A Raspberry Pi daemon to drive a 32x16 red/green LED matrix. These things
arrive as a kit, so some careful surface mount soldering skills are needed.

![Image of LED Matrix](images/s-l1600.jpg)

This board should be able to simulate (with PWM or [BCM](http://www.batsocks.co.uk/readme/art_bcm_1.htm)) the
[red-green color space](https://en.wikipedia.org/wiki/RG_color_space) as below:

![Red-Green color space](images/200px-Redgreen.png)

## Pinouts

| Board Pin | Name | Remarks                                             | RPi Pin | RPi Function |
|:---------:|------|-----------------------------------------------------|:-------:|--------------|
| 1         | GND  | Ground                                              | 6       | GND          |
| 3         | GND  | Ground                                              | 6       | GND          |
| 5         | GND  | Ground                                              | 6       | GND          |
| 7         | OE   | 74HC595 Output Enable (Active Low)                  | 11      | BCM 17       |
| 9         | R    | data input for 74HC595 (RED section / 4\*74HC595)   | 19      | BCM 10       |
| 11        | VCC  | +5V Power                                           | 2       | 5V0          |
| 13        | GND  | Ground                                              | 6       | GND          |
| 15        | GND  | Ground                                              | 6       | GND          |
| 2         | A    | row select with 74HC138                             | 15      | BCM 22       |
| 4         | B    | row select with 74HC138                             | 16      | BCM 23       |
| 6         | C    | row select with 74HC138                             | 18      | BCM 24       |
| 8         | D    | row select with 74HC138                             | 22      | BCM 25       |
| 10        | G    | data input for 74HC595 (GREEN section / 4\*74HC595) | 21      | BCM 9        |
| 12        | VCC  | +5V Power                                           | 2       | 5V0          |
| 14        | STB  | 74HC595 Strobe / Data Latch                         | 24      | BCM 8        |
| 16        | SCK  | 74HC595 Clock Input                                 | 23      | BCM 11       |

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
