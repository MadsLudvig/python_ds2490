# Python_ds2490

### Description

Module for reading ibutton devices through the DS2490 chipset via usb. Uses pyusb and libusb



### Example usage

```python
from python_ds2490.master import ds2490

device = ds2490.DS2490Master()

while True:
	result = device.OneDeviceSearch()
	if result:
		print(hex(result))
		break

```
### Dependencies
* pyusb
* libusb

