.. index:: qs

.. _quick:

Quick start guide
-----------------

In this guide we used Ubuntu in order to use the PMOD-Huawei board. With the following commands you will be able to navigate on the internet via the PMOD-Huawei. These steps are equal for both version of the boards ME909s and MU709S2.

1. On the PMOD-Huawei board insert the antenna in **CN4** connector

2. Insert your SIM card in the slot located in the bottom layer of the PMOD-Huawei

3. Insert the jumper from **PIN2** and **PIN3** of the **SW1**

4. Connect the empire board into the PMOD-Huawei **CN6** connector

5. Connect the Empire board to the PC

6. When the **LED1** on the PMOD-Huawei will start to blink steadly every 1 second the module will be connected to the netowrk

7. Use minicom and connect on the **/dev/ttyACM0** baudrate: 115200, 8N1

8. If all works correctly sending the command *AT* the PMOD will reply with *OK*

9. Write this command followed by enter: 

*AT+CGDCONT=1,"IP","YOUR APN"*

Where *"YOUR APN"* is the **Access Point Name** of your SIM

10. Launch this AT command *ATDT*99#* then exit from minicom

11. With the following commands you will be able to navigate on the internet:

 | *sudo pppd ttyACM0 115200 nodetach noauth lock usepeerdns*
 | *sudo route add default ppp0*

12. Open your preferred browser and try to navigate

.. warning::

  remember to disable your wifi connection or LAN connection if they have access to the internet


.. note::

  If you want use Windows, connect the **Empire** board to the PC, you have to install the right driver downloading `LPCUSBlib_VirtualSerial.inf <_static/LPCUSBlib_VirtualSerial.inf>`_ file and installing it. In this way you will have the virtual com enabled in order to comunicate with the PMOD.
  In this guide we don't explain how to use the PMOD-Huawei with Windows.

