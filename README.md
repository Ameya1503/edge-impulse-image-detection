# Edge Impulse Image Classification Project

## Project Overview
This project demonstrates **basic image classification using Edge Impulse**.  
- Images of objects (dogs and cats) were captured using **Arduino Nano 33 BLE Sense**.  
- Edge Impulse was used for **dataset upload, AI labeling, and training the model**.  
- The model achieved **~90% classification accuracy** on this small dataset.  

> **Goal:** Learn how to deploy ML models on edge devices with a low-cost microcontroller and small datasets.  

---

## Dataset
The dataset contains images captured with the **Arduino Nano 33 BLE Sense**:  

| Label | Number of Images |
|-------|----------------|
| Dog   | 40             |
| Cat   | 10             |

**Example Images:**

![Dog example](docs/dog_example.jpg)  
![Cat example](docs/cat_example.jpg)  

> You can replace these images with the actual screenshots or dataset samples in your `docs/` folder.

---

## Workflow Diagram

```mermaid
flowchart TD
    A[Capture Images] --> B[Upload to Edge Impulse]
    B --> C[Label Dataset]
    C --> D[Train Model]
    D --> E[Deploy to Arduino Nano 33 BLE Sense]
    E --> F[Run Inference / Classification]

Dependencies / Setup
Hardware
Arduino Nano 33 BLE Sense
USB cable for connection to PC

Software
Node.js (latest stable recommended)
Visual Studio Code with C++ development tools
Arduino IDE / Arduino CLI
Edge Impulse CLI (npm install -g edge-impulse-cli)
Libraries
ArduinoBLE
Edge Impulse Arduino library
