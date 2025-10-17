# Fusionpact DevOps Gauntlet Challenge – SOP
**Name:** Vaishnavi Tikke  
**Date:** October 2025  
**Cloud:** AWS EC2  
**Tools:** Docker, GitHub Actions, Prometheus, Grafana, MySQL  

---

<img width="1920" height="1080" alt="Screenshot (616)" src="https://github.com/user-attachments/assets/82d8dd85-f6ea-4e60-aae8-208f4a0c2a3f" />
<img width="1920" height="1080" alt="Screenshot (616)" src="https://github.com/user-attachments/assets/f8c86998-b271-4f13-83d8-21dca11fa566" />
<img width="1920" height="1080" alt="Screenshot (618)" src="https://github.com/user-attachments/assets/24ed8ca2-bcca-4811-914d-ccdb6a9eb38b" />
<img width="1920" height="1080" alt="Screenshot (619)" src="https://github.com/user-attachments/assets/681be7f2-7fb4-4583-ae33-20b2ccae0f62" />
<img width="1920" height="1080" alt="Screenshot (620)" src="https://github.com/user-attachments/assets/c55fe721-e705-4e99-b0f5-30caa1ca75f3" />
<img width="1920" height="1080" alt="Screenshot (621)" src="https://github.com/user-attachments/assets/9f14d87f-429f-4b30-84b0-5a337ca29e62" />



## 🥇 Level 1 – Cloud Deployment
**Commands Executed**
```bash
git clone https://github.com/<username>/fusionpact-devops-challenge.git
docker-compose up --build
Verification
Application accessible at:

Frontend: http://<EC2-IP>:3000

Backend: http://<EC2-IP>:5000


🥈 Level 2 – Monitoring & Observability

Prometheus configured to scrape backend & cAdvisor metrics.
Grafana dashboards visualize CPU, Memory, and Request count.


🥉 Level 3 – CI/CD Automation

Automated via GitHub Actions:

Build Docker Images

Push to Docker Hub

Deploy on EC2 via SSH


✅ Data Persistence Verification

After container restart, MySQL data persisted due to bound volume:
/var/lib/mysql → mysql_data.

Command:

docker-compose down
docker-compose up -d
# Data remained intact

Conclusion

This project demonstrates:

End-to-end DevOps lifecycle

Cloud deployment

Observability setup

Automated CI/CD
