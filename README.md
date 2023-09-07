# Feather_RAK3172_Phy_PingPong
Porting the “SubGHz_Phy_PingPong” project (STM32Cube, NUCLEO-WL55JC) for the Feather_RAK3172 board.

**Software:**

Project “SubGHz_Phy_PingPong” taken from [STM32CubeWL Firmware Package v1.3.0](https://www.st.com/en/embedded-software/stm32cubewl.html).

**Hardware:**

The project is based on **[Teapot Feather RAK3172](https://www.pcbway.com/project/shareproject/Teapot_Feather_RAK3172_Low_cost_LoRaWAN_Development_Board_75935372.html) Low-cost LoRaWAN Development Board**.

<img src="https://pcbwayfile.s3.us-west-2.amazonaws.com/web/23/04/27/0424333547358.png" alt="case_open.jpg"  />

Github: **[Teapotlabs Feather RAK3172](https://github.com/teapotlaboratories/feather-rak3172)**

**Description:**

This project implements a Ping-Pong application between two Ping-Pong devices.

Feather RAK3172 boards were used as such devices.

The applications aims to show a simple RX/TX RF link between the two Ping-Pong devices, one will be called Ping the other will be called Pong.

By default, each Ping-Pong Device starts as a master and will transmit a "Ping" message, and then wait for an answer.

At start-up, each Ping-Pong Device has its blue LED blinking with a frequency of approximately 5 Hz.
When boards will synchronize (Tx window of one board aligned with Rx window of the other board) the Ping-Pong Devices will blink its blue LED with a frequency of approximately 1 Hz.
The first Ping-Pong Device receiving a "Ping" message will become a slave and answers the master with a "Pong" message.

Logs via hyper-terminal complement LEDs indicators.

