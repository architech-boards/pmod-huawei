.. PMODHuawei documentation master file

Welcome to PMOD-Huawei documentation!
=====================================


:Version: 1.00A
:Copyright: (C)2016 Avnet Memec Silica company
:Date: 12 Apr 2016
:Reference name: BAEPMOD-COM-019-A01 and BAEPMOD-COM-021-A01

PMOD-Huawei Solution
--------------------

.. image:: _static/logo_silica_huawei.jpg

.. image:: _static/board_on.jpg

*PMOD-Huawei*

.. index:: index

**INTRODUCTION**
----------------

PMOD-Huawei board has mounted an Huawei device with the possibility using SIM or eUICC interface. Using the **Empire** board it is possible send via virtual com AT commands. There are 2 version of this board:

- **BAEPMOD-COM-019-A01** with mounted **MU709s** device
- **BAEPMOD-COM-021-A01** with mounted **ME909s** devuce

BAEPMOD-COM-019-A01
-------------------

**MU709** family is high-quality designed HSPA+ module in small size and Huawei standard LGA form factor which specially for industrial-grade M2M applications such as vehicle telematics, tracking, mobile payment, industrial router, safety monitor and industrial PDAs.

Based on Huawei standard LGA technology, the M709 modules provide a smoothly path to Huawei LTE high-speed modules.

MU709 family supports 21.6Mbps downlink data rate, providing data and voice service under global GSM/GPRS/EDGE/WCDMA/HSDPA/HSUPA/HSPA+ networks. The module also include enhanced features like embedded TCP/IP stack, SMTP, FOTA, Jamming Detection, Netscan, CMUX, SSL, eCall, Huawei enhanced AT commands, cell lock, network monitoring, DTMF decoder, baud rate adaptation, multi PDP, SIM swap, .etc.

Features:


- Bands: HSPA+/UMTS dual-band 900/2100 MHz, GSM/GPRS quad-band 850/900/1800/1900 MHz
- Data Transfer Rate: Downlink:21.6 Mbps, Uplink: 5.76 Mbps
- Interface:
    - Antenna interface
    - 1*8 UART & 1*2 UART
    - USB 2.0 High speed
    - PCM Voice
    - SIM Interface (1.8V/3.0V)
    - eUICC
    - GPIOs
- Power Supply: 3.3 V

BAEPMOD-COM-021-A01
-------------------

**ME909s** is the first LTE cat4 module based on Hi-Silicon chipset. Which is high-quality designed LTE module in small size and Huawei standard LGA form factor, especially for industrial-grade M2M applications such as vehicle telematics, tracking, mobile payment, industrial router, safety monitor and industrial PDAs.

ME909s-821 supports 150Mbps downlink data rate, including enhanced features like FOTA, USSD and Huawei enhanced AT commands.

ME909s-821 supports China region LTE Bands including both FDD-LTE & TDD-LTE, and has two different form factor: LGA and Mini PCIe form factor.

Features:

- Bands: LTE (FDD): B1,B3,B8; LTE (TDD): B38, B39,B40,B41; DC-HSPA+/HSPA+/HSPA/UMTS : B1, B5, B8,B9; TD-SCDMA: B34, B39; EDGE/GPRS/GSM : 900/1800 MHz
- Data Transfer Rate: DC-HSPA+ :Downlink:42 Mbps, Uplink: 5.76 Mbps; LTE TDD: Downlink:112Mbps, Uplink: 10Mbps; LTE FDD: Downlink:150 Mbps, Uplink: 50 Mbps @Bandwidth 20M
- Interface:
    - Antenna interface
    - 145 pins LGA interface
    - UART
    - PCM Voice
    - SIM Card
    - LED
- Power supply: 3.3 V



Developement tools
******************

The **ME909s** and **MU709s** uart interface is implemented with the **Empire** board, follow instruction inside :ref:`quick`

Document references
*******************

The board reference documentation is available on:

- the `architech-board <http://architechboards.org>`_ website. 

- the `mu709s documentation <http://consumer.huawei.com/en/solutions/m2m-solutions/products/support/user-guides/mu709s-6-en.htm>`_

- the `me909s documentation <http://consumer.huawei.com/en/solutions/m2m-solutions/products/support/user-guides/me909s_821_en.htm>`_


Contents:

.. toctree::
   :maxdepth: 2

   qs
   hw

