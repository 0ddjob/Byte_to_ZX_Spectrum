# Byte_to_ZX_Spectrum
Converter board for the Belarusian ZX Spectrum clone called the Байт (Byte). <br>
 
This machine has an, ahem, excessive 96-pin connector called an СНП59-96 (SNP59).  This connector has three rows of 32 pins each and is *almost* the same as a DIN41612 connector ... except for the Soviet-era 2.5mm pin pitch (compared to Western 2.54mm).  <br>

So a DIN41612 connector will not work.  That's the first issue.<br>

The second issue is, of course, it's not a Spectrum edge connector so peripherals won't connect anyway.

![The problem](/Images/The_problem.jpeg)

Special notes "Connecting DivIDE to BYTE":
- Pin A25 from divIDE we connect to byte on which we send out a low romcs signal such as the pin A30:
- Cut pin 4 or 4/5 of the DD67 (555ИД7) chip from ground and solder a resistor (180Ω to 10kΩ)
- Use a cable to lead pin 4 or 4/5 to a free pin of the edge connector, e.g. A30
- ROMCS signal (A25) from DivIDE connect to pin A30

![ROMCS signal](/Images/zx_byte4.jpg)

Current status (28-Sept-2023):<br>
- Connectors and test boards have arrived<br>
- Not working with DivMMC - investigating<br>

![Test board](/Images/zx_byte1.jpg)
