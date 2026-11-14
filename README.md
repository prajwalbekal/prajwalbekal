# Hi, I'm Prajwal Bekal

*I make noisy sensors confess, controllers behave, and Python turn test data into something engineers can actually use.*

Mechatronics engineer finishing an **M.Eng. in Mechatronic and Cyber-Physical Systems** at Deggendorf Institute of Technology (March 2027). My master's thesis at the **University of Stuttgart IFF** with **Fraunhofer IPA** develops learning-based support strategies for a shoulder exoskeleton in a musculoskeletal digital twin (simulation), and I work there as a research assistant. B.E. in Mechanical Engineering, with industrial experience in steam-turbine structural and rotor-dynamic analysis.

![Status](https://img.shields.io/badge/Status-Open%20to%20full--time%20roles%20from%20April%202027-brightgreen)
![Focus](https://img.shields.io/badge/Focus-GNC%20%2F%20AOCS%20%7C%20Control%20%7C%20Simulation-2E7D32)
![Domain](https://img.shields.io/badge/Domain-State%20Estimation%20%7C%20Robotics%20%7C%20Test%20Engineering-0A66C2)
![Location](https://img.shields.io/badge/Location-Stuttgart%2C%20Germany-informational)

## What I Work On

- Attitude determination and control for small satellites: detumbling, pointing, momentum management
- State estimation: EKF / MEKF sensor fusion with gyro-bias estimation
- Control design: PID, LQR / LQG, rate-limited quaternion feedback, actuator saturation
- Robotics simulation: ROS 2, Gazebo, MuJoCo / MyoSuite, CAD-to-simulation pipelines
- Test-data analysis: multi-channel DAQ, filtering, FFT and fault-signature detection
- Verification: deterministic tests, requirement checks and CI for reproducible results

## Featured Projects

### [Small-Satellite AOCS & Formation-Flying Simulator](https://github.com/prajwalbekal/smallsat-aocs-sim)

End-to-end attitude and orbit control for a 6U-class small satellite, from tumble to nadir pointing.

- B-dot detumbling with magnetorquers (filtered field derivative): 7.1°/s tip-off rates damped in 0.64 orbits
- MEKF (attitude + gyro bias) with star tracker and gyro: 0.012° knowledge error (99th percentile), consistent with its 3σ bounds and with the analytical steady state
- Rate-limited quaternion PID on reaction wheels with magnetic momentum dumping: 0.037° pointing error (99th percentile)
- Two-satellite formation: discrete LQR on the Clohessy–Wiltshire model, 250 m → 100 m slot in 1.08 orbits for 0.18 m/s Δv
- Telemetry analysis against requirements, 20 pytest tests, GitHub Actions CI

### [Self-Balancing Two-Wheel Robot (ROS 2 + Gazebo)](https://github.com/prajwalbekal/self-balancing-slope-robot)

Simulation of a two-wheel self-balancing robot in ROS 2 Humble and Gazebo Classic.

- Robot description generated from a SolidWorks STEP export (xacro, `ros2_control` effort interface)
- Cascade-PD balance controller that climbs an 8° ramp and descends an 8° decline under control
- Documented tuning order, debug log and known sim-to-real gaps

### [GNC Engineering Portfolio](https://github.com/prajwalbekal/GUIDANCE-NAVIGATION-CONTROL)

Three from-scratch Guidance, Navigation, and Control projects.

- 3-axis attitude control simulator with quaternion dynamics and PID / LQR-style feedback
- Extended Kalman Filter for noisy IMU and GPS sensor fusion with `0.6911 m` position RMSE
- Arduino PID controller sketch with a desktop plant simulator for offline tuning
- Reproducible validation metrics for tracking error, RMSE, and stability

### [Rotating Component Test Data Analyser](https://github.com/prajwalbekal/rotating-component-test-analyser)

Automated multi-channel sensor analysis pipeline for rotating component test engineering.

- Processes vibration, force, torque, and temperature data
- Applies 4th-order Butterworth filtering and single-sided FFT analysis
- Detects 1x/2x/3x shaft harmonics and a `187 Hz` bearing-defect signature
- Generates a structured PDF test report with plots and pass/fail verdicts
- GitHub Actions CI, MIT licensed, deterministic and reproducible

## Technical Stack

`Python` `NumPy` `SciPy` `Pandas` `Matplotlib` `pytest` `MATLAB / Simulink` `C / C++` `ROS / ROS2` `Gazebo` `MuJoCo` `MyoSuite` `NVIDIA Isaac Sim` `PID / LQR / LQG` `EKF / MEKF` `Reinforcement learning (PPO)` `FFT` `DAQ workflows` `SolidWorks` `ANSYS` `Git / GitHub Actions` `Linux`

## Current Focus

Finishing my master's thesis (March 2027). Looking for full-time roles from April 2027 in GNC / AOCS, control engineering, robotics simulation and test engineering, in Germany and across Europe.

## Contact

- GitHub: [github.com/prajwalbekal](https://github.com/prajwalbekal)
- LinkedIn: [linkedin.com/in/prajwal-bekal-5117b1150](https://de.linkedin.com/in/prajwal-bekal-5117b1150)
- Email: `prajwalbekal9@gmail.com`
