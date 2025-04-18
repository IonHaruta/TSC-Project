# TSC - Project

## Diagrama bloc
Diagrama bloc a proiectului nostru prezintă conexiunile dintre senzorii folosiți, microcontrollerul ESP32-C6 și componentele auxiliare:

![Block Diagram](./block-diagram.png) <!-- imaginea se pune în folderul proiectului -->

## Prezentare generală

Acest proiect TSC constă într-un sistem integrat care monitorizează temperatura și umiditatea mediului înconjurător cu ajutorul unui senzor DHT22 și afișează datele în timp real pe un ecran OLED SSD1306. Controlul și logica sistemului sunt gestionate de microcontrollerul ESP32-C6, iar interacțiunea utilizatorului se face printr-un buton fizic. Toate componentele sunt alimentate prin USB și sunt integrate pe o placă PCB proiectată în Fusion 360.



## BOM (Bill Of Materials)

| Component       | Device                | Link                                                                 | Datasheet                                                                 |
|-----------------|-----------------------|----------------------------------------------------------------------|---------------------------------------------------------------------------|
| BOOT_BUTTON     | BUTTON_CUSYOMV1        | [Link](https://ro.mouser.com/ProductDetail/Panasonic/EVQ-P7L01P?qs=rJ%252BziJWpyszWhhNszc02jQ%3D%3D&_gl=1*xzqk3l*_ga*dW5kZWZpbmVk*_ga_15W4STQT4T*dW5kZWZpbmVk*_ga_1KQLCYKRX3*dW5kZWZpbmVk)     | [Datasheet](https://componentsearchengine.com/Datasheets/2/EVQP7L01P.pdf) |
| C1              | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C1_BAT          | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C1_BAT1         | EAGLE-LTSPICE_CC0402   | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C1_BAT2         | EAGLE-LTSPICE_CC0402   | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C2              | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C2_BAT          | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C3              | RCL_CPOL-EUCT3528      | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C4              | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C4_USB          | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C5              | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C5_USB          | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C6              | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C7              | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C8              | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C9              | EAGLE-LTSPICE_CC0402   | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C10             | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| C10_SUPERCAP    | CPH3225A               | [Link](https://ro.mouser.com/ProductDetail/Seiko-Semiconductors/CPH3225A?qs=3etwrb1wR%252BhUOph6lAO7eg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/360/Seiko_Instruments_MicroBattery_E_20230330_2024Jan_-3561061.pdf) |
| CHANGE_BUTTON   | BUTTON_CUSYOMV1        | [Link](https://ro.mouser.com/ProductDetail/Panasonic/EVQ-P7L01P?qs=rJ%252BziJWpyszWhhNszc02jQ%3D%3D&_gl=1*xzqk3l*_ga*dW5kZWZpbmVk*_ga_15W4STQT4T*dW5kZWZpbmVk*_ga_1KQLCYKRX3*dW5kZWZpbmVk)     | [Datasheet](https://componentsearchengine.com/Datasheets/2/EVQP7L01P.pdf) |
| C_DELAY         | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| D1              | USBLC6-2SC6Y           | [Link](https://ro.mouser.com/ProductDetail/STMicroelectronics/USBLC6-2SC6Y?qs=gNDSiZmRJS%2FOgDexvXkdow%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/389/usblc6_2sc6y-1852505.pdf) |
| D2              | ESP32_WROVER_AVX...SD0805S020S1R0_AVX_... | [Link](https://eu.mouser.com/ProductDetail/KYOCERA-AVX/SD0805S020S1R0?qs=jCA%252BPfw4LHbpkAoSnwrdjw%3D%3D) | [Datasheet](http://datasheets.avx.com/schottky.pdf) |
| D3              | MBR0530               | [Link](https://www.snapeda.com/parts/MBR0530/Onsemi/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/MBR0530/Onsemi/view-part/?ref=eda) |
| D4              | MBR0530               | [Link](https://www.snapeda.com/parts/MBR0530/Onsemi/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/MBR0530/Onsemi/view-part/?ref=eda) |
| D5              | MBR0530               | [Link](https://www.snapeda.com/parts/MBR0530/Onsemi/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/MBR0530/Onsemi/view-part/?ref=eda) |
| D6              | PGB1010603MR          | [Link](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) |
| D7              | ESP32_WROVER_AVX---SD0805S020S1R0_AVX_... | [Link](https://eu.mouser.com/ProductDetail/KYOCERA-AVX/SD0805S020S1R0?qs=jCA%252BPfw4LHbpkAoSnwrdjw%3D%3D) | [Datasheet](http://datasheets.avx.com/schottky.pdf) |
| D8              | PGB1010603MR          | [Link](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) |
| D9              | PGB1010603MR          | [Link](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) |
| D10             | PGB1010603MR          | [Link](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) |
| D11             | PGB1010603MR          | [Link](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) |
| D12             | PGB1010603MR          | [Link](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) | [Datasheet](https://www.snapeda.com/parts/PGB1010603MR/Littelfuse/view-part/?ref=eda) |
| EPD_C1          | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| EPD_C2          | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| EPD_C5          | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| EPD_C6          | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| EPD_C7          | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| EPD_C8          | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| EPD_C9          | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| EPD_C10         | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| EPD_C11         | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| EPD_C12         | ESP32_WROVER_EAGLE-LTSPICE_CC0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/CC0402MRX5R5BB106?qs=zEY9bCHj09eCmUJdZuS5Lg%3D%3D)  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf) |
| IC1             | BD5229G-TR            | [Link](https://ro.mouser.com/ProductDetail/ROHM-Semiconductor/BD5229G-TR?qs=4kLU8WoGk0vvnhrrYwdszw%3D%3D) | [Datasheet](https://fscdn.rohm.com/en/products/databook/datasheet/ic/power/voltage_detector/bd52xxg-e.pdf) |
| IC4             | XC6220A331MR-G        | [Link](https://ro.mouser.com/ProductDetail/Torex-Semiconductor/XC6220A331MR-G?qs=AsjdqWjXhJ8ZSWznL1J0gg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/760/xc6220-3371556.pdf) |
| J1              | FH34SRJ-24S-0.5SH_99_ | [Link](https://ro.mouser.com/ProductDetail/Hirose-Connector/FH34SRJ-24S-0.5SH99?qs=vcbW%252B4%252BSTIpKBl5ap9J8Fw%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/185/FH34SRJ_24S_0_5SH_99__CL0580_1255_6_99_2DDrawing_0-1615044.pdf) |
| J2              | USB4110-GF-A          | [Link](https://ro.mouser.com/ProductDetail/GCT/USB4110-GF-A?qs=KUoIvG%2F9IlYiZvIXQjyJeA%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/837/GCT_USB4110_Product_Drawing___20k_cycles-3455479.pdf) |
| J3              | QWIIC_CONNECTORJS-1MM | [Link](https://ro.mouser.com/ProductDetail/SparkFun/PRT-14417?qs=wd5RIQLrsJhgdz%2FpmZ%2F3GQ%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/813/Qwiic_Connector_Datasheet-1223982.pdf) |
| J4              | 112A-TAAR-R03_ATTEND  | [Link](https://store.comet.srl.ro/Catalogue/Product/43497/) | [Datasheet](https://store.comet.srl.ro/Catalogue/Product/43497/) |
| L1              | 744043680IND_4828-WE-TPC_WRE | [Link](https://ro.mouser.com/ProductDetail/Wurth-Elektronik/744043680?qs=PGXP4M47uW6VkZq%252BkzjrHA%3D%3D) | [Datasheet](https://eu.mouser.com/ProductDetail/Wurth-Elektronik/744043680?qs=PGXP4M47uW6VkZq%252BkzjrHA%3D%3D) |
| PFMF.050.1      | ESP32C6_VARISTORCN1812 | [Link](https://ro.mouser.com/ProductDetail/KEMET/VE1812K401R050?qs=OycAS1CGnlizCtaoDVbQTA%3D%3D) | [Datasheet](https://www.mouser.co.uk/ProductDetail/EPCOS-TDK/B72520T0350K062?qs=dEfas%2FXlABIszF52uu7vrg%3D%3D) |
| Q1              | DMG2305UX-7           | [Link](https://ro.mouser.com/ProductDetail/Diodes-Incorporated/DMG2305UX-7?qs=L1DZKBg7t5F%2FNBHrjfxC%252Bg%3D%3D) | [Datasheet](https://www.diodes.com/assets/Datasheets/DMG2305UX.pdf) |
| Q2              | ESP32_WROVER_SPARKFUN-DISCRETESEMI_MOSFET_... | [Link](https://ro.mouser.com/ProductDetail/Diodes-Incorporated/DMG2305UX-7?qs=L1DZKBg7t5F%2FNBHrjfxC%252Bg%3D%3D) | [Datasheet](https://www.diodes.com/assets/Datasheets/DMG2305UX.pdf) |
| Q3              | D8                    | [Link](https://ro.mouser.com/ProductDetail/Vishay-Semiconductors/SI1308EDL-T1-GE3?qs=bX1%252BNvsK%2FBramh9tgpOaEw%3D%3D) | [Datasheet](https://componentsearchengine.com/part-view/SI1308EDL-T1-GE3/Vishay) |
| R1              | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R1_PINH         | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R1_PINH1        | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R1_BAT          | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R1_PWRUSB       | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R2              | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R2_PINH         | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R2_PINH1        | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R2_USB          | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R2_USB1         | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R2_BAT          | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R3              | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R4              | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R5              | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R6              | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R7              | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R8              | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R9              | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R10             | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| RESET_BUTTON    | BUTTON_CUSYOMV1        | [Link](https://ro.mouser.com/ProductDetail/Panasonic/EVQ-P7L01P?qs=rJ%252BziJWpyszWhhNszc02jQ%3D%3D&_gl=1*xzqk3l*_ga*dW5kZWZpbmVk*_ga_15W4STQT4T*dW5kZWZpbmVk*_ga_1KQLCYKRX3*dW5kZWZpbmVk)     | [Datasheet](https://componentsearchengine.com/Datasheets/2/EVQP7L01P.pdf) |
| R_BOOT          | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R_CAPACITOR     | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R_CHANGE        | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R_CL1           | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| R_RESET         | ESP32_WROVER_EAGLE-LTSPICE_RR0402 | [Link](https://ro.mouser.com/ProductDetail/YAGEO/RC0402FR-07100KL?qs=mnq%2FyloZIXzTlUn7JAHSWg%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/447/YAGEO_PYu_RC_Group_51_RoHS_L_12-3313492.pdf) |
| SENSOR2         | ESP32_WROVER_BME680_BME680 | [Link](https://ro.mouser.com/ProductDetail/Bosch-Sensortec/BME680?qs=v271MhAjFHjo0yA%2FC4OnDQ%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/783/BST_BME680_DS001-1509608.pdf) |
| SJ1             | SJ                     | [Link](https://grabcad.com/library/solder-jumpers-1)                | [Datasheet](https://grabcad.com/library/solder-jumpers-1)                |
| TP1 - TP17      | TPTP20R               | -                                                               | -                                                                    |
| U1              | W25Q512JVEIQ          | [Link](https://ro.mouser.com/ProductDetail/Winbond/W25Q512JVEIQ?qs=l7cgNqFNU1jw6svr3at6tA%3D%3D)     | [Datasheet](https://ro.mouser.com/datasheet/2/949/Winbond_W25Q512JV_Datasheet-3240039.pdf) |
| U2              | ESP32-C6-WROOM-1-N8   | [Link](https://ro.mouser.com/ProductDetail/Espressif-Systems/ESP32-C6-WROOM-1-N8?qs=8Wlm6%252BaMh8ST02Gmwp74cw%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/891/Espressif_ESP32_C6_WROOM_1__Datasheet_V0_1_PRELIMI-3239987.pdf) |
| U3              | DS3231SN#             | [Link](https://ro.mouser.com/ProductDetail/Analog-Devices-Maxim-Integrated/DS3231SN?qs=1eQvB6Dk1vhUlr8%2FOrV0Fw%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/609/DS3231-3421123.pdf) |
| U4              | MAX17048G+T10         | [Link](https://ro.mouser.com/ProductDetail/Analog-Devices-Maxim-Integrated/MAX17048G%2bT10?qs=D7PJwyCwLAoGnnn8jEPRBQ%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/609/MAX17048_MAX17049-3469099.pdf) |
| U5              | ESP32_WROVER_SPARKFUN-IC-POWER_MCP73831 | [Link](https://ro.mouser.com/ProductDetail/Microchip-Technology/MCP73831T-2ACI-OT?qs=yUQqVecv4qvbBQBGbHx0Mw%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/268/MCP73831_Family_Data_Sheet_DS20001984H-3441711.pdf) |



## ⚙️ Descriere hardware

Acest proiect utilizează un microcontroller **ESP32-C6** pentru gestionarea unui sistem de afișare și citire senzorială:

- **DHT22** transmite date despre temperatură și umiditate către ESP32-C6 prin pinul digital.
- **Display-ul OLED SSD1306** este conectat pe magistrala I2C pentru a afișa datele în timp real.
- **Butonul push** este utilizat pentru resetarea valorilor sau declanșarea anumitor moduri.
- Sistemul este alimentat prin USB 5V, iar consumul total este estimat la ~120mA.

## Pini utilizați pe ESP32-C6

| Componentă             | Pin ESP32-C6 | Motiv utilizare           |
|------------------------|--------------|----------------------------|
| DHT22                  | GPIO4        | Intrare digitală de la senzor |
| OLED SSD1306 (SCL)     | GPIO8        | Comunicație I2C - clock     |
| OLED SSD1306 (SDA)     | GPIO9        | Comunicație I2C - date      |
| Buton push             | GPIO3        | Input digital               |

## Tabel pini ESP32-C6

| Pin ESP32-C6 | Utilizare             | Componentă asociată      |
|--------------|------------------------|---------------------------|
| GPIO0        | neutilizat             | -                         |
| GPIO1        | neutilizat             | -                         |
| GPIO2        | neutilizat             | -                         |
| GPIO3        | Input                  | Buton push                |
| GPIO4        | Intrare digitală       | DHT22                     |
| GPIO5        | neutilizat             | -                         |
| GPIO6        | neutilizat             | -                         |
| GPIO7        | neutilizat             | -                         |
| GPIO8        | I2C Clock (SCL)        | OLED SSD1306              |
| GPIO9        | I2C Data (SDA)         | OLED SSD1306              |
| GPIO10       | neutilizat             | -                         |
| GPIO11       | neutilizat             | -                         |
| GPIO12       | neutilizat             | -                         |
| GPIO13       | neutilizat             | -                         |
| GPIO14       | neutilizat             | -                         |
| GPIO15       | neutilizat             | -                         |
| GPIO16       | neutilizat             | -                         |
| GPIO17       | neutilizat             | -                         |
| GPIO18       | neutilizat             | -                         |
| GPIO19       | neutilizat             | -                         |
| GPIO20       | neutilizat             | -                         |



## Conectarea componentelor

- **DHT22**: Pinul de semnal al senzorului este conectat la **GPIO4**. Alimentarea senzorului este făcută de la 3.3V și GND.
- **Display OLED SSD1306**: Conectat la magistrala I2C:
  - SCL -> **GPIO8**
  - SDA -> **GPIO9**
- **Butonul fizic**: Legat între **GPIO3** și GND, folosind rezistență pull-up internă activată în cod.
- **Alimentare**: Proiectul este alimentat prin USB (5V), cu stabilizator pe placă pentru 3.3V.



## Alte observații

- Design-ul PCB a fost realizat în Fusion 360 PCB și randarea este disponibilă în fișierul `rendering.png`.
- Componentele au fost amplasate compact, ținând cont de răcire și accesibilitate.

