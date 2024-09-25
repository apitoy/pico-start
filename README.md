# pico-start
How to start?


## **What is Raspberry Pi Pico?**


![Raspberry Pi Pico Installing UF2 MicroPython Firmware](https://github.com/user-attachments/assets/84344e90-688c-4bad-8586-660d0c42e623)

The Raspberry Pi Pico is more than just a microcontroller board; it’s a gateway to the vast and exciting world of physical computing. Developed by the renowned Raspberry Pi Foundation, the Pico stands out as a compact powerhouse that enables makers, hobbyists, educators, and professionals to bring their digital ideas into the tangible world. This remarkable device is built around the RP2040 microcontroller, a groundbreaking piece of technology that’s been meticulously designed in-house by the Raspberry Pi team. This decision to create their own microcontroller chip signifies the Foundation’s commitment to providing a highly optimized, powerful, and yet accessible platform for all levels of users.

Despite its modest dimensions, the Raspberry Pi Pico is a marvel of engineering, boasting impressive technical capabilities. At its core lies the dual-core Arm Cortex-M0+ processor, a highly efficient yet powerful CPU that can handle a multitude of tasks ranging from simple LED control to complex data processing. Accompanying this processor is 264KB of SRAM, providing sufficient space for running your programs, and 2MB of onboard Flash memory, ideal for storing your code and essential data.


![Raspberry Pi Pico Installing UF2 MicroPython Firmware](https://github.com/user-attachments/assets/bfbb8aa0-fe80-4509-bbc1-48bb83075c25)

## LED Blink program

Once you have everything set up, it’s time to write your first program. If you’re new to programming, don’t worry – Raspberry Pi Pico is beginner-friendly. You can start with MicroPython, a beginner-friendly programming language that’s easy to learn.

MicroPython allows you to write code in a simplified version of Python, making it accessible to beginners. You can use the Thonny IDE, which comes pre-installed with the Raspberry Pi Pico software, or any other software a per your choice to write and run your programs.

```python
from machine import Pin
import utime
 
# Define the onboard LED pin
led = Pin(25, Pin.OUT)
 
while True:
    led.value(1)  # Turn LED on
    utime.sleep(1) # Wait for 1 second
    led.value(0)  # Turn LED off
    utime.sleep(1) # Wait for 1 second
```
