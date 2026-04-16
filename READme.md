# Network Utilization Monitor using SDN (POX + Mininet)

## 📌 Problem Statement

To monitor network bandwidth utilization using Software Defined Networking by collecting flow statistics and calculating real-time bandwidth.

## ⚙️ Tools Used

* Mininet
* POX Controller
* OpenFlow
* Ubuntu

## 🧠 Approach

* Created topology using Mininet
* Implemented POX controller to collect flow statistics
* Calculated bandwidth using byte count differences over time
* Displayed utilization in real-time

## ▶️ Steps to Run

1. Start POX controller:

   ```
   ./pox.py forwarding.l2_learning misc.monitor
   ```

2. Start Mininet:

   ```
   sudo mn --controller=remote --topo single,3
   ```

3. Test connectivity:

   ```
   pingall
   ```

4. Generate traffic:

   ```
   h1 ping h2
   ```

## 📊 Output

* Displays bandwidth for each flow in Bytes/sec
* Example:

  ```
  Flow 10.0.0.1 -> 10.0.0.2 | Bandwidth: 114.96 Bytes/s
  ```

## 📸 Screenshots

(Attach all screenshots here)

## ✅ Conclusion

Successfully monitored network utilization using SDN controller with real-time bandwidth calculation.
