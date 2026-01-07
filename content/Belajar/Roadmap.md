---
cssclasses:
- cheatsheet
---
## 0. Prasyarat: Fondasi Awal

- **Konsep Dasar Jaringan & Sistem Komputer** #card-teal
    
    - Apa itu IP Address, DNS, HTTP/HTTPS, dan port.
        
    - Cara kerja sistem operasi secara umum.
        

# Tahapan Roadmap

## 1. Pahami Kultur & Filosofi DevOps

Ini adalah langkah paling fundamental menurutku. Tanpa memahami "mengapa"-nya, semua _tools_ yang akan kupelajari nanti tidak akan ada artinya.

- **Konsep Inti:** #card-blue
    
    - **C.A.L.M.S. Framework:** Culture, Automation, Lean, Measurement, Sharing.
        
    - **The Three Ways:** Prinsip aliran kerja, _feedback loops_, dan kultur eksperimen & pembelajaran berkelanjutan.
        
    - **Breaking Down Silos:** Kolaborasi erat antara tim Development (Dev) dan Operations (Ops).
        
- **What to do:** #card-blue
    
    - **Membaca buku:** _The Phoenix Project_ (wajib!), _The DevOps Handbook_.
        
    - **Memahami tujuan utama**: Meningkatkan kecepatan, kualitas, dan keandalan rilis perangkat lunak.
        

## 2. Kuasai Sistem Operasi (Wajib: Linux)

Hampir semua infrastruktur modern berjalan di atas Linux.

- **Manajemen Command Line (CLI):** #card-green
    
    - **Navigasi & File:** `ls`, `cd`, `pwd`, `cp`, `mv`, `rm`, `mkdir`, `find`, `grep`, `sed`, `awk`.
        
    - **Permission:** `chmod`, `chown`.
        
    - **Manajemen Proses:** `ps`, `top`, `htop`, `kill`, `nice`.
        
- **Manajemen Jaringan:** #card-green
    
    - `ip` atau `ifconfig`, `netstat`, `ss`, `ping`, `traceroute`, `curl`, `wget`.
        
- **Manajemen Paket & Scripting:** #card-green
    
    - **Debian/Ubuntu:** `apt`, `apt-get`.
        
    - **CentOS/RHEL/Fedora:** `yum`, `dnf`.
        
    - **Shell Scripting (Bash):** Otomatisasi tugas-tugas repetitif.
        

## 3. Bahasa Pemrograman & Scripting

- **Bahasa & Konsep Kunci:** #card-yellow
    
    - **Python (Sangat Direkomendasikan):** Serbaguna, banyak _library_ untuk cloud (seperti `boto3`).
        
    - **Go (Baik untuk Diketahui):** Banyak _tools_ DevOps modern (Docker, K8s) dibuat dengan Go.
        
    - **Pahami:** REST API, JSON, dan YAML.
        

## 4. Git - Version Control System (VCS)

- **Perintah & Konsep:** #card-red
    
    - **Dasar:** `git init`, `add`, `commit`, `push`, `pull`, `clone`.
        
    - **Branching:** `branch`, `checkout`, `merge`. Pahami alur kerja **Git Flow** atau **GitHub Flow**.
        
    - **Lanjutan:** `rebase`, `cherry-pick`, `stash`.
        
- **Platform:** #card-red
    
    - Biasakan diri dengan **GitHub**, **GitLab**, atau **Bitbucket**.
        

## 5. CI/CD - Continuous Integration & Delivery

- **Konsep Kunci:** #card-purple
    
    - **Continuous Integration (CI):** Setiap perubahan kode otomatis di-_build_ dan diuji.
        
    - **Continuous Delivery (CD):** Hasil dari CI otomatis disiapkan untuk rilis ke produksi.
        
    - **Continuous Deployment:** Hasil dari CI otomatis dirilis ke produksi.
        
- **Tools Populer:** #card-purple
    
    - **GitLab CI/CD:** Modern, terintegrasi erat dengan GitLab.
        
    - **GitHub Actions:** Sangat populer, ekosistem luas.
        
    - **Jenkins:** Sangat kuat dan fleksibel, kurva belajar lebih curam.
        

## 6. Infrastructure as Code (IaC) & Manajemen Konfigurasi

Mendefinisikan infrastruktur (server, db, jaringan) menggunakan kode.

- **Provisioning (Membuat Infrastruktur):** #card-orange
    
    - **Terraform:** Standar industri, deklaratif, mendukung banyak _cloud provider_.
        
- **Configuration Management (Mengkonfigurasi Server):** #card-orange
    
    - **Ansible:** Populer, _agentless_, mudah dipelajari (menggunakan YAML).
        

## 7. Containerization & Orchestration

Mengubah cara mengemas dan menjalankan aplikasi.

- **Containerization Engine:** #card-pink
    
    - **Docker:** Standar de-facto. Pelajari `Dockerfile`, `docker build`, `docker run`, `docker-compose`.
        
- **Container Orchestration:** #card-pink
    
    - **Kubernetes (K8s):** Platform orkestrasi paling dominan.
        
    - **Konsep Kunci:** `Pod`, `Service`, `Deployment`, `ConfigMap`, `Secret`, `Ingress`.
        
    - **Tools Pendukung:** `kubectl` (CLI), `Helm` (Package Manager).
        

## 8. Monitoring, Logging, & Observability

Kita tidak bisa memperbaiki sesuatu yang tidak bisa kita lihat.

- **Monitoring (Metrics):** #card-teal
    
    - **Prometheus:** Mengumpulkan metrik (CPU, RAM, dll.).
        
    - **Grafana:** Memvisualisasikan metrik dalam bentuk _dashboard_.
        
- **Logging (Events):** #card-teal
    
    - **ELK/EFK Stack:** Elasticsearch, Logstash/Fluentd, Kibana.
        
- **Tracing (Requests):** #card-teal
    
    - **Jaeger / Zipkin:** Melacak alur _request_ melalui _microservices_.
        

## 9. Cloud Providers

Pilih salah satu untuk didalami layanan intinya.

- **Pilihan Utama & Layanan Inti (Contoh AWS):** #card-blue
    
    - **Penyedia:** AWS, GCP, Azure.
        
    - **Compute:** EC2, Lambda.
        
    - **Storage:** S3, EBS.
        
    - **Networking:** VPC, Route 53.
        
    - **Database:** RDS, DynamoDB.
        
    - **IAM:** Identity and Access Management.
        

## 10. Keamanan - DevSecOps

Mengintegrasikan keamanan ke dalam setiap fase siklus pengembangan.

- **Konsep & Praktik:** #card-red
    
    - **SAST:** Menganalisis kode sumber (Contoh: SonarQube).
        
    - **DAST:** Menguji aplikasi yang sedang berjalan.
        
    - **Secret Management:** Gunakan **HashiCorp Vault** atau fitur bawaan _cloud_.
        
    - **Container Security:** Pindai _image_ untuk kerentanan (Contoh: Trivy, Clair).