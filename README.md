# <p align="center">项目说明</p>

- 基于HAL库的USB虚拟串口，通过串口通讯控制单片机生成对应占空比的PWM波形，用于控制共地的无刷电调器。
- TB上HLK的无刷电调，启动前需要设置Compare为`<500`（官方要求频宽0.2ms但是貌似只要小于1ms即可），如需设置其他Compare值才启动成功，可能是由于Period和Prescaler设置不同，请自行测试。
- ![Logic Analyzer](./Snipaste_2025-07-04_16-59-12.png)
