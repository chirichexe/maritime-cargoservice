# Maritime CargoService

Project for **Software Systems Engineering M** (A.Y. 2025/2026) – University of Bologna.

Distributed system to automate container loading operations in a ship's cargo hold.

## Architecture & Components

* **CargoService:** Business logic orchestrator implemented via custom DSL actors.
* **CargoRobot:** Differential Drive Robot (DDR) adapter for physical container handling.
* **IOPort:** Web GUI (Javalin, WebSockets, CoAP) for customer interaction.
* **Periphery:** ESP32 node (MicroPython) driving Sonar and LED via MQTT.

## Tech Stack

* **Core & Domain:** Custom DSL, Kotlin, Java
* **Protocols:** MQTT (Mosquitto), CoAP (Observe), WebSockets
* **Infrastructure:** Docker, Docker Compose, PyTest

## Engineering Focus

* **Hexagonal Architecture:** Domain logic strictly isolated from hardware and protocols via adapters.
* **Actor-Based Messaging:** Asynchronous message-passing (`Dispatch`, `Request`, `Reply`, `Event`) over shared state.
* **Iterative Refinement:** Incremental substitution of Sprint 1 mocks with Sprint 2 physical/web peripherals without domain changes.

## Documentation

| Sprint | Documents |
| :--- | :--- |
| **Sprint 0** | [v1](sprint0/docs/sprint0_v1.pdf) · [v2](sprint0/docs/sprint0_v2.pdf) · [v3](sprint0/docs/sprint0_v3.pdf) |
| **Sprint 1** | [v1](sprint1/docs/sprint1_v1.pdf) · [v2](sprint1/docs/sprint1_v2.pdf) |
| **Sprint 2** | [v1](sprint2/docs/sprint2_v1.pdf) |

## Team

* **Davide Chirichella**
* **Gabriele Doti**
* **Daniele Maccagnan**
