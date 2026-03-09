------------------------------------------
Coela Can't! Protogen LED Board V1 Manufacturing Files
Document Version: V1.0
------------------------------------------
Included are design and manufacturing files to get LED boards ordered and shipped right to your door ready to use! You will need to order from JLCPCB or another SMT assembly service to manufacture the PCBs and assemble the boards. Directions for ordering from JLCPCB are included.

With these boards, you can utilize my ProtoTracer software to use raytracing to render live graphics that can react to your voice, motion, or transition smoothly between different face shapes just like VRChat avatars - it even uses FBX files! Don't worry the software is free and can be found here: https://github.com/coelacant1/ProtoTracer

The 3D STEP CAD files are included, so if the design is not exactly what you want then you have the ability to modify and tweak it! This design is built around printing on the Prusa i3 MK3s with build dimensions of X:250mm, Y:210mm, and Z:210mm. This design can be printed on smaller printers but may need to be modified or split requiring glue or the addition of screw mounts.


------------------------------------------
ASSEMBLY
------------------------------------------
Parts list:
Threaded insert kit (M2, M3, M4, M5): https://www.amazon.com/DYWISHKEY-Knurled-Threaded-Embedment-Assortment/dp/B07MWBJB67/ref=sr_1_2?crid=32CP64EBTXEPU&keywords=metric+threaded+inserts&qid=1642454449&sprefix=metric+threaded+inserts%2Caps%2C65&sr=8-2
M2 Screws: https://www.amazon.com/uxcell-M2x6mm-Thread-Button-Socket/dp/B01B1OD9UQ/ref=sr_1_3?crid=3FN0QLAWPNBSN&keywords=m2x6+screws&qid=1642454542&sprefix=m2x6+screws%2Caps%2C74&sr=8-3

The rear LED board mount will be attached using M2 threaded inserts into the frame and M2x6mm screws for the cover and mount.


------------------------------------------
VISOR
------------------------------------------
Print the V1 or V2 Buck
Make a vacuum former tutorial: https://www.youtube.com/watch?v=Gx66mS7U2vY
Material: Use 0.04" or 1.0mm PETG for proper thickness 


------------------------------------------
3D Printing
------------------------------------------
Recommended build dimensions: 250mmx210mmx210mm
Resolution: 0.2mm or higher quality
Supports: Not necessary at high resolution, except for jaw.
Brim: Depending on your build surface a brim may be needed to bed adhesion
Material: PETG for frame - PLA can be used but it can melt if left in hot areas or in vehicles

Two STL files are available, the Flat version is to be used if 1.6mm boards are used for production. The Bend version can be used with 0.8mm boards and thinner.

------------------------------------------
Electronics
------------------------------------------
Controller:
Teensy 4.0: https://www.pjrc.com/store/teensy40.html
OctoWS2811 LED Controller for the Teensy 4.0: https://www.pjrc.com/store/octo28_adaptor.html

Power: 
USB-C Decoy Trigger (USB-C to set voltage out): https://www.amazon.com/Type-C-USB-C-charge-trigger-detector/dp/B07T6LPP9W/ref=sr_1_3?crid=2FWFKCTMHJGR&keywords=usb+c+trigger&qid=1642455379&sprefix=usb+c+trigger%2Caps%2C71&sr=8-3
Buck Converter (5v-38V input to 5V output): https://www.amazon.com/Pololu-Step-Down-Voltage-Regulator-D24V90F5/dp/B01M9C9Q1E
Recommend 20W+ USB-C PD battery

Provide 5V directly to the LED boards from the buck converter and the signal lines from the OctoWS2811 controller.

------------------------------------------
Software
------------------------------------------
Software for controlling the head can be found at: https://github.com/coelacant1/ProtoTracer
To use this, include the ProtoV2Controller.h as the primary controller and pick the animation to display on the face from the animations class. Use the KaiborgV1 animation as a default protogen face.
