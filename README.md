# ESP32 FreeRTOS Tutorial Collection

This repository collects a series of ESP32 projects demonstrating **FreeRTOS fundamentals** using the **Arduino framework** on **PlatformIO**.  
Each submodule focuses on a distinct real-time concept-from basic multitasking to modular and event-driven systems.

## Project Index

| Order | Project | Description |
|-------|----------|-------------|
| 1 | [`esp-freertos-task`](https://github.com/royyandzakiy/esp-freertos-task) | Core FreeRTOS concepts: tasks, priorities, queues, semaphores, and core pinning. |
| 2 | [`esp-freertos-timer-statemachine`](https://github.com/royyandzakiy/esp-freertos-timer-statemachine) | Event-driven state machine using FreeRTOS queues and software timers. |
| 3 | [`esp-freertos-eventgroups`](https://github.com/royyandzakiy/esp-freertos-eventgroups) | Synchronization and signaling using FreeRTOS Event Groups. |
| 4 | [`esp-freertos-sensor-led-wifi`](https://github.com/royyandzakiy/esp-freertos-sensor-led-wifi) | Modular system architecture combining tasks for sensor, LED, and WiFi management. |
| 5 | [`esp-rtos-event-loop`](https://github.com/royyandzakiy/esp-rtos-event-loop) | ESP IDF Native event loop library with events and queues. |
| 6 | [`esp-rtos-esp-timer`](https://github.com/royyandzakiy/esp-rtos-esp-timer) | ESP IDF Native timer library with start/stop, periodics, debugging. |
| 7 | [`esp-rtos-debugging`](https://github.com/royyandzakiy/esp-rtos-debugging) | FreeRTOS Debugging Utilities |
| 8 | [`esp-rtos-failure`](https://github.com/royyandzakiy/esp-rtos-failure) | <WIP> FreeRTOS Runtime Error Simulator: Stack Overflow, Memory Corruption, Deadlocks, etc. |

## Getting Started

Each submodule is a self-contained PlatformIO project.

To clone all modules:

```bash
git clone git@github.com:royyandzakiy/esp-freertos-tutorial.git
git submodule update --init --recursive
```

Then open any folder (e.g., `esp-freertos-task/`) in **VSCode with PlatformIO**, build, and upload to your ESP32 board.

## Requirements

- **Board:** ESP32 / ESP32-S3 DevKitC  
- **Framework:** Arduino (via PlatformIO)  
- **Tool:** Visual Studio Code + PlatformIO extension  

## Notes

Each project:
- Uses FreeRTOS primitives in isolation for clarity.  
- Runs on standard ESP32 boards without external hardware.  
- Includes inline comments and serial output for easy observation.  

More modules may be added as the series expands (e.g., message buffers, stream buffers, and real hardware integration).