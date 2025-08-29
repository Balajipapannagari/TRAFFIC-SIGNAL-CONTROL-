# TRAFFIC-SIGNAL-CONTROL-
Density -based Adaptive Traffic Signal Control For Efficient Junction Clearence.

Traffic congestion at urban intersections is a major challenge, often caused by conventional traffic
signal systems that follow fixed time cycles irrespective of real-time conditions. This project
proposes a density-based adaptive traffic signal control system that dynamically adjusts the
green light duration based on the number of vehicles waiting in each lane. The system captures
traffic data using cameras or sensors, counts vehicles in real-time through computer vision
techniques, and assigns signal clearance time proportional to the detected traffic volume. If a lane
has more vehicles, the system increases green time to clear the congestion; if a lane has fewer
vehicles, the system reduces the clearance time and allocates the extra time to busier lanes.
This ensures fair distribution of green signals, reduces idle waiting, and minimizes overall delay at
the junction. The project integrates OpenCV-based vehicle detection, simple decision algorithms
(like max-pressure or longest-queue-first), and a simulation/implementation framework (e.g.,
SUMO simulator or Arduino-based signal model). Expected outcomes include reduced average
waiting time, shorter queues, and smoother traffic flow compared to fixed-time systems. This
work demonstrates a cost-effective and scalable solution that can be applied to smart city traffic
management, providing a foundation for future extensions such as emergency vehicle
prioritization, public transport preference, and AI-driven predictive control.



Project Plan (Step-by-Step)
1 Problem Definition: Traditional traffic lights = fixed cycle, inefficient. Need adaptive control
based on vehicle density.

2 Data Collection: Method A: Camera + OpenCV/YOLO for vehicle counting. Method B: Sensors
(IR/Ultrasonic) for low-cost prototype.

3 Vehicle Detection & Counting: Implement image processing (OpenCV) to count cars in each
lane. Maintain queue length data per lane in real-time.

4 Decision Algorithm: If (Queue length is high) → Allocate longer green time. If (Queue length is
low) → Allocate shorter green time. Ensure fairness (no starvation of smaller lanes).

5 Signal Control Implementation: Arduino/NodeMCU with LEDs for traffic signal prototype OR
SUMO/Matlab simulation for traffic flow.

6 Evaluation Metrics: Average waiting time per vehicle, Average queue length, Signal utilization
efficiency.

7 Extensions (Future Scope): Emergency vehicle detection (ambulance priority), Integration
with IoT (cloud-based monitoring), AI/ML model for predictive traffic flow
