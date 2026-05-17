# Build-A-USB-Hub
A modular USB hub with jumper pins to connect everything featuring a SL2.1A chip! It will feature: USB A connector modules, USB C Port Modules which could be used for hub data input or data output, and SL2.1A modules to split 1 USB input into 4 outputs.

<img width="416" height="332" alt="image" src="https://github.com/user-attachments/assets/451f23ab-128b-4cea-bfc8-a2f0fef11fea" />

<img width="315" height="329" alt="image" src="https://github.com/user-attachments/assets/584e61c7-32b8-4c99-bff7-2522b7051468" />

<img width="427" height="332" alt="image" src="https://github.com/user-attachments/assets/01b36a76-57f8-42b0-a4af-0b71380126ef" />

<img width="373" height="390" alt="image" src="https://github.com/user-attachments/assets/b11a6dc0-e37e-4a55-8b47-37b872c94da6" />

# *Why, just <ins>why</ins>?*

I LOVE designing circuit boards and making random tech. So, I thought of making a USB hub, but <ins>modular</ins>. And I also thought, why not also turn it into a USB-A to USB-C adapter as well since it was modular. So, I made a unique design that has pins on the modules that made them removable. You could even stack the modules that convert 1 USB port into 4! And when you just need a adapter to connect you USB-C device to a USB-A port (or the other way around!), you could just remove the modules and connect them to each other! **I mean, just think about it, *have you seen a modular USB hub (where the modules could turn into adapters)?***

<img width="340" height="309" alt="image" src="https://github.com/user-attachments/assets/67eead2a-3f3a-4691-a990-63596ebe53ec" />

<img width="415" height="605" alt="image" src="https://github.com/user-attachments/assets/fd8e1a38-d4c1-479b-83fb-c1e14fb471ff" />

<img width="480" height="585" alt="image" src="https://github.com/user-attachments/assets/69fa61f4-e154-43ae-8d14-5d254ed8cacf" />

<img width="442" height="635" alt="image" src="https://github.com/user-attachments/assets/8b20ce0f-3ef2-4e43-a665-459ceaf7e57b" />

# BOM

These will be the parts needed to build my project:

| Name | Purpose | Quantity | Total Cost (USD) | Link | Distributor |
|---|---|---|---|---|---|
| PCBs | These will be the PCBs for all of my modules! | 4 | 14.30 | https://jlcpcb.com/ | JLCPCB |
| USB-231-ARY | These will be the USB-A output ports for my USB-A output module! | 5 | 0.88 | https://www.lcsc.com/product-detail/C720525.html?spm=wm.gwc.xh.6.cbm___wm.mxq.ssl.gwc&lcsc_vid=ElEMAldVRFYLX1VfQlldXwBUFAMIVFRWQlhdVV0ET1kxVlNRT1ZXU11RRVJaXzsOAxUeFF5JWBEcCEoDFhIXAgAHWQIBCks%3D | LCSC |
| KH-TYPE-C-CY-14P | This will be the USB port on my USB-C modules which can be used as both an input from the host for the hub or as an output! | 10 | 4.31 | https://www.lcsc.com/product-detail/C2919655.html?spm=wm.gwc.xh.5.cbm___wm.mxq.ssl.gwc&lcsc_vid=ElEMAldVRFYLX1VfQlldXwBUFAMIVFRWQlhdVV0ET1kxVlNRT1ZXU11RRVJaXzsOAxUeFF5JWBEcCEoDFhIXAgAHWQIBCks%3D | LCSC |
| MF1/4W-5.1KΩ±1% T | This will be the resistor that will pull the CC pins on the USB-C module to ground to avoid conflicts in connecting devices! | 50 | 0.56 | https://www.lcsc.com/product-detail/C119340.html?spm=wm.gwc.xh.4.cbm___wm.mxq.ssl.gwc&lcsc_vid=ElEMAldVRFYLX1VfQlldXwBUFAMIVFRWQlhdVV0ET1kxVlNRT1ZXU11RRVJaXzsOAxUeFF5JWBEcCEoDFhIXAgAHWQIBCks%3D | LCSC |
| AM90 | This will be the male USB port that will plug into the host USB port! | 10 | 0.70 | https://www.lcsc.com/product-detail/C404965.html?spm=wm.gwc.xh.3.cbm___wm.mxq.ssl.gwc&lcsc_vid=ElEMAldVRFYLX1VfQlldXwBUFAMIVFRWQlhdVV0ET1kxVlNRT1ZXU11RRVJaXzsOAxUeFF5JWBEcCEoDFhIXAgAHWQIBCks%3D | LCSC |
| NSR0320MW2T1G | This will be the diode that will prevent current backflow back into the USB port the hub is connected to! | 20 | 2.34 | https://www.lcsc.com/product-detail/C48192.html?spm=wm.gwc.xh.2.cbm___wm.mxq.ssl.gwc&lcsc_vid=ElEMAldVRFYLX1VfQlldXwBUFAMIVFRWQlhdVV0ET1kxVlNRT1ZXU11RRVJaXzsOAxUeFF5JWBEcCEoDFhIXAgAHWQIBCks%3D | LCSC |
| SL2.1A | This will be the chip that converts 1 USB input into 4 outputs! | 5 | 1.34 | https://www.lcsc.com/product-detail/C6798314.html?spm=wm.gwc.xh.1.cbm___wm.mxq.ssl.gwc&lcsc_vid=ElEMAldVRFYLX1VfQlldXwBUFAMIVFRWQlhdVV0ET1kxVlNRT1ZXU11RRVJaXzsOAxUeFF5JWBEcCEoDFhIXAgAHWQIBCks%3D | LCSC |
| CL10A106KP8NNNC | These will be the capacitors that will keep the voltage stable for my USB hub! | 100 | 1.03 | https://www.lcsc.com/product-detail/C19702.html?spm=wm.gwc.dh.0.cbm___wm.mxq.ssl.gwc&lcsc_vid=ElEMAldVRFYLX1VfQlldXwBUFAMIVFRWQlhdVV0ET1kxVlNRT1ZXU11RRVJaXzsOAxUeFF5JWBEcCEoDFhIXAgAHWQIBCks%3D | LCSC |
