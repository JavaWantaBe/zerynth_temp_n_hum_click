.. module:: TempHumClick

================
Temp & Hum click
================

This module contains the :class:`TempHumClick` carries STs HTS221
temperature and relative humidity sensor. Its highlight is that it
outputs its measurement in a 16-bit resolution and has a high
rH sensitivity of 0.004% (although the accuracy range. In comparison,
HTU21D click, HDC1000 click and SHT1x click all output a 12-14 bit
resolution signal.

**Resources**

* Datasheet: http://www.st.com/st-web-ui/static/active/en/resource/technical/document/datasheet/DM00116291.pdf

* Product Page: http://www.mikroe.com/click/temp-hum/

* Product Manual: http://www.mikroe.com/downloads/get/2383/temp_hum_click_user_manual_v100.pdf

    
.. class:: TempHumClick

    Creates an intance of a new TempHumClick.

    :param drvsel: I2C Bus used `( I2C0, I2C0 )`
    :param int_pin: Interrupt pin used for events
    :param address: Slave address, default 0x5f
    :param clk: Clock speed, default 400kHz

    :Example:

.. code-block:: python

    temp_hum = tempnhum_click.TempHumClick( I2C1,D31 )
    temp, hum = temp_hum.get_temp_humidity()

    
.. method:: get_temp_humidity()

        Retrieves both temperature and humidity in one call.

        returns temp, humidity

        
