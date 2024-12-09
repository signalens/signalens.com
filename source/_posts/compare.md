---
title: Comparison
permalink: /compare/
hide: true
sticky: 100
---

## Specification between different SDRs

The comparison table presents a comprehensive overview of various software-defined radio (SDR) devices, including the SignalSDR series, AntSDR models, RTL-SDR, PlutoSDR, Ettus products, BladeRF versions, LimeSDR, and HackRF One. It compares key specifications such as frequency range, interface types, RF bandwidth, sample depth, sample rate, number of transmitter and receiver channels, duplex capabilities, programmable logic resources, chipsets used, open-source status, GPSDO availability, oscillator precision, transmit power, and pricing.

The table highlights the diverse range of SDR options available in the market, varying in capabilities and price points. Devices like the SignalSDR series offer wide frequency ranges and high bandwidths, competing with more established brands. Entry-level options like RTL-SDR provide basic functionality at a low cost, while high-end devices from Ettus offer advanced features for professional use. The comparison reveals trade-offs between frequency coverage, processing power, interface options, and price across different SDR platforms, allowing users to choose based on their specific requirements and budget constraints.

<style>
  table {
    width: 100%;
    border-collapse: collapse;
  }
  th, td {
    padding: 8px 12px;
    border: 1px solid #ddd;
    text-align: left;
  }
  th {
    background-color: #f2f2f2;
    position: sticky;
    top: 0;
    z-index: 2;
  }
  td:first-child, th:first-child {
    position: sticky;
    left: 0;
    background-color: #f2f2f2;
    z-index: 1;
  }
  table th {
    background-color: #f8f8f8;
  }
</style>

| **Model**               | **Frequency Range**    | **Ethernet** | **USB**            | **Debug**              | **I-PEX**                     | **GPIO**          | **Additional Boot Option** | **RF Bandwidth** | **Sample Depth** | **Sample Rate** | **Channels/Duplex**           | **Logic Gates**      | **Chipset** | **GPSDO**    | **Oscillator Precision**           | **Transmit Power**                         |
|---------------------|--------------------|----------|----------------|--------------------|---------------------------|---------------|------------------------|--------------|--------------|-------------|---------------------------|------------------|----------|----------|--------------------------------|----------------------------------------|
| **SignalSDR Pro**       | 70 MHz - 6 GHz     | Gigabit  | Type-B, OTG    | USB-TTL / USB-JTAG | CLOCK IN, CLOCK OUT, TRIG | Full 40 pins  | SD Card / Flash / JTAG | 61.44 MHz    | 12 bits      | 61.44 MSPS  | 2 Tx / 2 Rx / Full Duplex | 85k              | AD9361   | Yes      | ~ 1 ppm                        | Up to 10 dBm (depending on frequency)  |
| **RTL-SDR**             | 500 KHz - 1766 MHz | N/A      | Type-A 2.0     | N/A                | N/A                       | N/A           | N/A                    | 3.2 MHz      | 8 bits       | 3.2 MSPS    | 0 Tx / 1 Rx / No Duplex   | N/A              | RTL2832U | No       | ~ 1 ppm                        | N/A                                    |
| **PlutoSDR**            | 325 MHz - 3.8 GHz  | N/A      | Micro 2.0, OTG | N/A                | N/A                       | N/A           | N/A                    | 20 MHz       | 12 bits      | 61.44 MSPS  | 2 Tx / 2 Rx / Full Duplex | 28k              | AD9363   | No       | ~ 20 ppm                       | Up to 6 dBm (depending on frequency)   |
| **Ettus B200**          | 70 MHz - 6 GHz     | N/A      | Type-B         | N/A                | N/A                       | Minimun pins  | N/A                    | 61.44 MHz    | 12 bits      | 61.44 MSPS  | 1 Tx / 1 Rx / Full Duplex | 75k              | AD9364   | External | ~2 ppm                         | 10 dBm+                                |
| **Ettus B210**          | 70 MHz - 6 GHz     | N/A      | Type-B         | N/A                | N/A                       | Minimun pins  | N/A                    | 61.44 MHz    | 12 bits      | 61.44 MSPS  | 2 Tx / 2 Rx / Full Duplex | 100k             | AD9361   | External | ~2 ppm                         | 10 dBm+                                |
| **Ettus B205mini**      | 70 MHz - 6 GHz     | N/A      | Micro          | N/A                | N/A                       | Minimun pins  | N/A                    | 61.44 MHz    | 12 bits      | 61.44 MSPS  | 1 Tx / 1 Rx / Full Duplex | 150k             | AD9364   | External | ~2 ppm                         | 10 dBm+                                |
| **BladeRF x40/x115**    | 300 MHz - 3.8 GHz  | N/A      | Type-B         | N/A                | N/A                       | Minimun pins  | N/A                    | 40 MHz       | 12 bits      | 40 MSPS     | 1 Tx / 1 Rx / Full Duplex | 40k (115k avail) | LMS6002M | No       | ~ 1 ppm                        | 6 dBm                                  |
| **BladeRF 2.0 xA4/xA9** | 70 MHz - 6 GHz     | N/A      | Type-B         | N/A                | N/A                       | Minimun pins  | N/A                    | 56 MHz       | 12 bits      | 61.44 MSPS  | 2 Tx / 2 Rx / Full Duplex | 32k (292k avail) | AD9361   | No       | ~ 1 ppm                        | 8 dBm                                  |
| **LimeSDR mini 2.0**    | 10 MHz - 3.5 GHz   | N/A      | Type-A         | N/A                | N/A                       | Minimun pins  | N/A                    | 40 MHz       | 12 bits      | 30.72 MSPS  | 1 Tx / 1 Rx / Full Duplex | 44k              | LMS7002M | No       | ~1 ppm initial, ~ 4 ppm stable | Up to 10 dBm (depending on frequency)  |
| **AntSDR E200 AD9363**  | 325 MHz - 3.8 GHz  | Gigabit  | N/A            | USB-TTL            | 2(TX2/RX2)                | Minimun pins  | SD Card                | 20 MHz       | 12 bits      | 61.44 MSPS  | 2 Tx / 2 Rx / Full Duplex | 85k              | AD9363   | No       | ~2 ppm                         | Up to 10 dBm (depending on frequency)  |
| **AntSDR E200 AD9361**  | 70 MHz - 6 GHz     | Gigabit  | N/A            | USB-TTL            | 2(TX2/RX2)                | Minimun pins  | SD Card                | 56 MHz       | 12 bits      | 61.44 MSPS  | 2 Tx / 2 Rx / Full Duplex | 85k              | AD9361   | No       | ~2 ppm                         | Up to 10 dBm (depending on frequency)  |
