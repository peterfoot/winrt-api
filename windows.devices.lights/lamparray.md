---
-api-id: T:Windows.Devices.Lights.LampArray
-api-type: winrt class
ms.custom: RS5
---

<!-- Class syntax.
public class LampArray 
-->

# Windows.Devices.Lights.LampArray

## -description
Represents a LampArray device attached the system.  Currently, only [HID LampArrays](https://www.usb.org/sites/default/files/hutrr84_-_lighting_and_illumination_page.pdf) are supported.
## -remarks
LampArray devices have one or more lamp indexes (for example, lights/LEDs/bulbs, etc…) whose color state can be directly manipulated.  Static information (retrieved from the device) describe supported colors, geometric positions and intended purposes for each lamp index.

These devices can be found as part of composite devices (for example, keyboard with RGB lighting) or as standalone.

An application can set lamp state at any time, but state will only be applied by the system while application is in focus.

LampArrays are enumerated by [DeviceWatcher](../windows.devices.enumeration/devicewatcher.md), and retrieved via [FromIdAsync](lamparray_fromidasync_1322863552.md).

## -see-also

[LampArrayKind](lamparraykind.md), [Lighting and Illumination](https://www.usb.org/sites/default/files/hutrr84_-_lighting_and_illumination_page.pdf), [Dynamic lighting](/windows/uwp/devices-sensors/lighting-dynamic-lamparray)

## -examples

[AutoRGB Sample](https://github.com/microsoft/Dynamic-Lighting-AutoRGB)

Demonstrates how to extract a single, representative color from a desktop screen and use it to illuminate LED lamps on a connected RGB device.
