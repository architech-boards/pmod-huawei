.. index:: hardware

.. _hardware:

Hardware Guide
--------------

The board is provided with:

- PMOD-Huawei

Configuration MU709S2
*********************

The MU709S2 works with auto-baudrate or baudrate fixed:
- auto-baudrate: the first time you sent a data to the device, it will set its baudrate as yours.
- The device starts with a fixed baudrate and it sends data about its configuration

We have configurated the device with baudrate fixed in this way:

0. Connect the board with the PC via USB

1. Launch minicom and set the baudrate to **9600**

2. Send a charachter

3. Send the command: *AT+IPR=115200*

4. Turn off the module and set the minicom to **115200**, then turn on the module

5. Set these commands to configure the LED timing:

*AT^LEDCTRL=2,00000FF0,1,20,2*
*AT^LEDCTRL=2,0000000F,1,2,20*

Useful general AT Commands
**************************

- **AT+GMR**: permits to know the firmware version. Actually the version is **11.652.65.00.00**
- **AT+CPIN?**: if MU709S2/ME909S replies with *READY*, the SIM (or the eUICC) is correctly seen
- **AT+CSQ**: it is used to check the quality of the signal:

====== =================================
<rssi> GSM or UTRAN Cell Signal Strength
====== =================================
0      ≤ –113 dBm
WCDMA  1 –111 dBm
2      –30 –109 dBm to –53 dBm
31     ≥ –51 dBm
99     Unknown or undetectable
====== =================================


Datasheet and more
******************

Please refer to:

- the `architech-board <http://architechboards.org>`_ website. 

- the `mu709S2 documentation <http://consumer.huawei.com/en/solutions/m2m-solutions/products/support/user-guides/mu709s-6-en.htm>`_

- the `me909s documentation <http://consumer.huawei.com/en/solutions/m2m-solutions/products/support/user-guides/me909s_120_en.htm>`_

.. image:: _static/logo_architech.jpg

