# สรุปความรู้เรื่อง GitHub และ DevOps

GitHub คือแพลตฟอร์ม Git-based สำหรับจัดเก็บและจัดการซอร์สโค้ด (Version Control) ส่วน DevOps คือวัฒนธรรม แนวปฏิบัติ และชุดเครื่องมือที่ผสานงานระหว่างฝั่งพัฒนา (Development) และฝั่งดูแลระบบ (Operations) เพื่อส่งมอบซอฟต์แวร์ได้รวดเร็ว เสถียร และปลอดภัยยิ่งขึ้น

1. สรุปภาพรวม Git & GitHub

Git (Local): ระบบ Distributed Version Control บันทึกประวัติการแก้ไขโค้ด ทำงานแบบออฟไลน์บนเครื่องนักพัฒนา

GitHub (Cloud): พื้นที่เก็บโค้ดส่วนกลาง (Remote Repository) ที่เพิ่มฟีเจอร์การทำงานร่วมกัน:

Pull Request (PR) & Code Review: ตรวจสอบโค้ด อภิปราย และอนุมัติก่อนรวมเข้า Branch หลัก

Branching Strategy: แบ่งสายการทำงาน (เช่น GitFlow หรือ Trunk-based) เพื่อไม่ให้โค้ดใหม่กระทบระบบที่ใช้งานจริง

Issue Tracking & Projects: จัดการบั๊ก วางแผนงานแบบ Kanban Board

2. แกนหลักของ DevOps (Core Practices)

CI/CD (Continuous Integration / Continuous Delivery & Deployment): รวมโค้ดเข้าส่วนกลางบ่อยๆ ทดสอบอัตโนมัติ และปล่อยขึ้นระบบอย่างต่อเนื่อง

Infrastructure as Code (IaC): จัดการโครงสร้างพื้นฐานเซิร์ฟเวอร์ด้วยโค้ด (เช่น Terraform, Ansible)

Microservices & Containerization: แยกแอปพลิเคชันเป็นส่วนย่อย บรรจุลงคอนเทนเนอร์ (เช่น Docker, Kubernetes) เพื่อความยืดหยุ่นในการสเกล

Monitoring & Observability: ติดตามประสิทธิภาพ ตรวจจับข้อผิดพลาด และดู Log แบบเรียลไทม์ (เช่น Prometheus, Grafana)

DevSecOps: แทรกการตรวจสอบความปลอดภัยเข้าไปในทุกขั้นตอนตั้งแต่การเขียนโค้ด

3. จุดเชื่อมโยง: GitHub ในฐานะฟันเฟืองของ DevOps

GitHub พัฒนาจากแค่ที่ฝากโค้ดมาเป็นแพลตฟอร์ม DevOps ครบวงจร (End-to-End DevOps Platform):

GitHub Actions: เครื่องมือ CI/CD Engine ในตัว กำหนด Workflow ด้วยไฟล์ YAML สำหรับ Build, Test, และ Deploy ไปยัง Cloud (AWS, GCP, Azure) อัตโนมัติทันทีที่มีการ Push หรือเปิด PR

GitHub Packages: คลังจัดเก็บ Software Artifacts หรือ Docker Images

GitHub Advanced Security: ตรวจจับช่องโหว่ (CodeQL/SAST), ตรวจจับ API Keys ที่เผลอหลุด (Secret Scanning) และแจ้งเตือน Library ที่มีช่องโหว่ (Dependabot)