# Honeypot Attack Visualization with Grafana

This project presents a personal cybersecurity experiment where I deployed a **Cowrie honeypot** on an **AWS EC2 instance**, collected attack logs, and visualized them with **Grafana**.  
The aim was to better understand real-world SSH brute-force attacks, practice cloud deployment, and build a monitoring/visualization workflow.

---

## 🔎 What I Did
- Deployed a **Cowrie SSH Honeypot** on AWS (Ubuntu EC2).
- Collected and stored logs of real-world attacks.
- Configured **Grafana** dashboards to visualize:
  - Number of connection attempts
  - Top attacker IPs
  - Command usage by attackers
  - Time-based attack patterns
- Secured access with Grafana’s sharing features (no public exposure of AWS).

---

## 🛠️ Technologies Used
- **AWS EC2** – to host the honeypot
- **Cowrie Honeypot** – SSH/Telnet medium-interaction honeypot
- **Grafana** – data visualization
- **Docker** (optional, for local Grafana instance)
- **Linux system administration** (systemd, SSH hardening, security groups)

---

## 📚 What I Learned
- Setting up a honeypot in the cloud
- Handling and securing log data
- Using Grafana for security analytics
- Applying good practices for **cloud security** (not exposing sensitive dashboards directly)
- Dockerizing tools for reproducibility

---

## 📊 Demo Dashboard
You can view the demo dashboard here (read-only shared link):

👉 [Grafana Shared Dashboard](http://localhost:3000/goto/kuOv95rNR?orgId=1)

*(This is a public Grafana Cloud share link with limited read-only access)*

---

## 🚀 Run Grafana Locally 
In order to access the dashboard shared publicly it is needed to Run a Grafana instance locally on port 3000. As such here is a simple way to achieve this with the following commands:

```bash
git clone git@github.com:loickballoy/HonePot-With-Cowrie-On-AWS.git
cd grafana-honeypot-visualization

# Launch Grafana on localhost:3000
docker run -d -p 3000:3000 grafana/grafana
```
Then open the shared link above in your browser.

---

## 📄 Note

This project is for educational and  demonstration purposes only. Running a honeypot in production without proper precations can expose your insfrastructure.

## 👤 Author

Developed by Balloy Loïck – Computer Engineering student at EPITA (SSSE Major).

- Portfolio: [portfolio-link]

- GitHub: [https://github.com/loickballoy]

- LinkedIn: [https://www.linkedin.com/in/loick-balloy-332708203/]