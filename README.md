# ☸️ Kube Surfer — Kubernetes Deployment Endless Runner

**Kube Surfer** is a 3D Kubernetes-themed endless runner web game inspired by *Subway Surfers*, built with **Three.js** and the **Web Audio API**. Play as a **K8s DevOps Captain** racing across a high-speed server-rack highway, dodging real-world cluster failures, collecting running Pods, and scaling your deployment to production!

---

## 🎮 Gameplay Overview

Step into the boots of a Cloud-Native Captain equipped with a Kubernetes helm-wheel helmet and container jetpack. Your mission is to keep the cluster healthy by surviving production incidents and scaling through 5 progressive Kubernetes deployment stages.

### ✨ Key Features
* **3D Server-Rack Highway:** Dynamic chase camera, neon data lanes, and glowing server towers built using Three.js.
* **Synthesized Sound Effects:** Retro arcade sound effects generated natively using the Web Audio API (no external audio files required).
* **Responsive Controls:** Supports both Desktop keyboard controls and Mobile touch swipe gestures.
* **Progressive Deployment Levels:** Speed and difficulty dynamically scale as your cluster matures.

---

## 🕹️ Controls

| Action | Desktop (Keyboard) | Mobile (Touch) |
| :--- | :--- | :--- |
| **Move Left** | `Left Arrow` or `A` | Swipe Left |
| **Move Right** | `Right Arrow` or `D` | Swipe Right |
| **Jump** | `Up Arrow`, `W`, or `Space` | Swipe Up |
| **Slide / Roll** | `Down Arrow` or `S` | Swipe Down |

---

## 🚧 Cluster Obstacles & Power-Ups

### ⚠️ Obstacles (Production Incidents)
* **`CrashLoopBackOff` Barriers:** Red ground barriers — **Jump** over them.
* **`OOMKilled (137)` Beams:** Overhead memory-limit blockers — **Slide** underneath them.
* **`502 Bad Gateway` Firewalls:** Full-height blocked nodes — **Switch lanes** to avoid.
* **`DDoS Flood` Trains:** Fast-moving incoming traffic waves — **Switch lanes** quickly.

### ⚡ Collectibles & Power-Ups
* **☸️ Kubernetes Pods:** Collect Pods to boost your deployment score and replica count.
* **🧲 Helm Chart Magnet:** Automatically pulls nearby Pods from all three lanes toward you.
* **🛡️ HPA Autoscaler Shield:** Protects your Captain from one fatal cluster crash and smashes right through obstacles.

---

## 📈 Deployment Stages (Levels)

As your distance and score increase, your cluster automatically promotes through 5 deployment stages:

1. **Level 1 — `kubectl apply`:** Initial manifest deployment at standard speed.
2. **Level 2 — `ReplicaSet Ready`:** Pods spin up and cluster speed increases.
3. **Level 3 — `Ingress Routed`:** External traffic hits the cluster with denser obstacle patterns.
4. **Level 4 — `HPA Autoscaling`:** High-velocity scaling mode under heavy load.
5. **Level 5 — `Multi-Region HA Mesh`:** Maximum speed and ultimate production resilience challenge.

---

## 🛠️ Tech Stack

* **Frontend:** HTML5, CSS3 (Glassmorphism UI)
* **3D Graphics Engine:** Three.js (WebGL)
* **Audio:** Web Audio API (Procedural sound synthesis)
* **Deployment Ready:** Single-file static architecture (`kube-surfer.html`) — easily hostable on **GitHub Pages**, **AWS S3 + CloudFront**, **Nginx**, or inside a **Kubernetes Pod**.

---

## 🚀 How to Run Locally or Deploy on Kubernetes

### 1. Run Locally
Simply open `kube-surfer.html` in any modern web browser, or serve it via Python:
```bash
python3 -m http.server 8080
