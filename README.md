# SPCN-012
1. Hypervisor Technology
-คือเทคนิคการจำลองให้ระบบปฏิบัติการหลายระบบสามารถทำงานพร้อมกันบนโฮสต์ได้ ใช้ประโยชน์ได้สูงสุด จำลองระบบปัฏิบัติการ แบบมัลติคอร์มัลติเธรด และ Ram จำนวนมาก เหมาะสำหรับเมนเฟรมมากกว่า windown OS เพราะ Hypervisor-
-Hypervisor (ไฮเปอร์ไวเซอร์) มีกี่ประเภท
hypervisor มีกี่ประเภท? หลายคนอาจสงสัยกันอยู่ โดยส่วนมากแล้ว Hypervisor จะมีอยู่ด้วยกัน 2 ประเภท ได้แก่ Type 1 hypervisor (Baremetal Architectur) และ Type 2 hypervisor (Hosted Architecture)

Hypervisor Type 1 (Baremetal Architectur)
Hypervisor รูปแบบนี้จะทำงานโดยตรงบนฮาร์ดแวร์ของเซิร์ฟเวอร์ ดังนั้นไม่ต้องใช้ระบบปฏิบัติการอื่นเพื่อที่จะใช้ Hypervisor นี้ ตัวอย่างของ Hypervisor Type 1 ได้แก่ VMware ESXi หากดูจากเทคนิคการจำลองเสมือนในการใช้ฮาร์ดแวร์ VMware ESXi จะถือว่าเป็น Hypervisor Type 1

Hypervisor Type 2 (Hosted Architecture)
Hypervisor รูปแบบนี้จะทำหน้าที่เป็นซอฟต์แวร์ซึ่งจัดการและใช้เครื่องเสมือน ถ้าต้องการเข้าถึงทรัพยากรฮาร์ดแวร์จะต้องผ่านระบบปฏิบัติการก่อน 

อ้างอิง : https://personet.co.th/hypervisor/

2. Container Technology
-คือการจัดเก็บแอพพลิเคชั่นให้อยู่ในรูปแบบที่ง่ายต่อการโยกย้ายและนำขึ้นระบบ (deploy) โดยประกอบไปด้วยตัวแอพพลิเคชั่นเอง library หรือ binary ต่าง ๆที่จำเป็นในการรันแอพพลิเคชั่นนั้นๆ และการกำหนดค่าต่างๆ ของแอพพลิเคชั่นนั้น ๆ เพราะฉะนั้นไม่ว่าจะย้ายตัวแอพพลิเคชั่นที่ถูกจัดเก็บเป็น container ไปรันที่ไหน จะสามารถทำงานได้เหมือนเดิมโดยไม่คำนึงถึงระบบปฏิบัติการ-

อ้างอิง : https://blog.cloudhm.co.th/from-monolithic-to-microservice/

3. Monolithic MicroService
-คือการเขียน Software ที่รวมทุกอย่างไว้ที่จุดจุดเดียว อาจเป็นระบบก้อนเดียว หรือ Server เครื่องเดียว จะเขียนด้วย Framework อะไรก็แล้วแต่ แต่สุดท้ายคือ รวมไว้ที่เดียวกัน มี Model Service Database ข้อดี ของแบบนี้คือมันเขียนง่าย คนเดียวก็เขียนได้ ไม่มีความซับซ้อน และตรงไปตรงมา ดูแลในระยะสั้นง่าย เหมาะกับระบบที่ไม่ซับซ้อน หรือมีแผนการพัฒนาในระยะยาววางไว้แล้ว-

-ข้อจำกัด-
-ม้เราพยายามใช้ Framework เดียวกัน แต่ในรายละเอียดปลีกย่อยต่างๆ Dev ต่างทีม ต่างบริษัทก็จะมีวิธีแก้ปัญหาต่างกัน ซึ่งเมื่อมีการเปลี่ยนมือ หรือแม้กระทั่งทีมเดิมเข้ามาดู Code ที่เคยเขียนไปหลายๆปี ยังไงซะ ก็ต้องมานั่งไล่ดู Code -
-ทุกษาต่างมีสิ่งที่ทำเก่งต่างกัน ทีนี้เมื่อเราต้องทำฟังชันที่ภาษาที่ใช้ในปัจจุบันไม่เก่ง เราก็ต้อง “ดันทุรัง” ทำทุกวิธีให้ทำให้ได้ สุดท้ายก็ลงเอยด้วยวิธี Tricky ต่าง บางครั้งแปลกๆ ซึ่ง Tricky มากเท่าไหร่มัน ไม่ดีแน่ในการดูแลระยะยาว นั่นคือความเสถียรในระบบนั้นก็จะลดลงตาม-


อ้างอิง : https://blog.cloudhm.co.th/from-monolithic-to-microservice/

4. Proxmox
เป็นแพลตฟอร์มการจัดการเซิร์ฟเวอร์โอเพ่นซอร์ซที่สมบูรณ์แบบสำหรับการจำลองเสมือนขององค์กร ได้รับการพัฒนาโดย Proxmox Server Solutions ในออสเตรียภายใต้ Internet Foundation of Austria และเผยแพร่ภายใต้ GNU General Public License

อ้างอิง :https://www.quickserv.co.th/knowledge-base/technology/VMware-vSphere-%e0%b8%81%e0%b8%b1%e0%b8%9a-Proxmox-%e0%b8%aa%e0%b8%b3%e0%b8%ab%e0%b8%a3%e0%b8%b1%e0%b8%9a%e0%b8%98%e0%b8%b8%e0%b8%a3%e0%b8%81%e0%b8%b4%e0%b8%88-%e0%b9%83%e0%b8%8a%e0%b9%89%e0%b9%81%e0%b8%9a%e0%b8%9a%e0%b9%84%e0%b8%ab%e0%b8%99%e0%b8%94%e0%b8%b5%e0%b8%97%e0%b8%b5%e0%b9%88%e0%b8%aa%e0%b8%b8%e0%b8%94/#:~:text=Proxmox%20%E0%B8%84%E0%B8%B7%E0%B8%AD%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3%3F,%E0%B9%83%E0%B8%95%E0%B9%89%20GNU%20General%20Public%20License

5. Ceph
เป็นระบบistributed storage แบบหนึ่ง หรือพูดง่ายๆ คือ เป็น storage ที่ทำงานบน cluster ของ computer node โดยในระบบ Ceph Storage ประกอบไปด้วย node 3 ประเภท คือ Monitor ทำหน้าที่ดูแลสถานะของ cluster. OSD (Object Storage Device) ทำหน้าที่อ่าน/เขียนข้อมูลตามคำสั่งของผู้ใช้

อ้างอิง :https://www.throughwave.co.th/2017/04/10/%E0%B9%81%E0%B8%99%E0%B8%B0%E0%B8%99%E0%B8%B3-ceph-storage-distributed-storage-%E0%B8%A3%E0%B8%B9%E0%B8%9B%E0%B9%81%E0%B8%9A%E0%B8%9A%E0%B9%83%E0%B8%AB%E0%B8%A1%E0%B9%88%E0%B8%97%E0%B8%B5%E0%B9%88/#:~:text=Ceph%20Storage%20%E0%B9%80%E0%B8%9B%E0%B9%87%E0%B8%99%E0%B8%A3%E0%B8%B0%E0%B8%9A%E0%B8%9A%20distributed,%E0%B8%84%E0%B8%B3%E0%B8%AA%E0%B8%B1%E0%B9%88%E0%B8%87%E0%B8%82%E0%B8%AD%E0%B8%87%E0%B8%9C%E0%B8%B9%E0%B9%89%E0%B9%83%E0%B8%8A%E0%B9%89

6. NFS
Network File System หรือเรียกย่อ ๆ ว่า NFS เป็น Protocol ที่ช่วยให้ Computer สามารถแชร์ข้อมูลผ่าน Network ได้ มีการพัฒนาและนำมาใช้งานใน ปี ค.ศ.1984 และยังเป็น Solution ที่ยังคงใช้งานกันแพร่หลายจวบจนปัจจุบัน

อ้างอิง : https://blog.cloudhm.co.th/nfs-vs-smb/#:~:text=NFS%20%E0%B8%84%E0%B8%B7%E0%B8%AD%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3%3F,%E0%B9%81%E0%B8%9E%E0%B8%A3%E0%B9%88%E0%B8%AB%E0%B8%A5%E0%B8%B2%E0%B8%A2%E0%B8%88%E0%B8%A7%E0%B8%9A%E0%B8%88%E0%B8%99%E0%B8%9B%E0%B8%B1%E0%B8%88%E0%B8%88%E0%B8%B8%E0%B8%9A%E0%B8%B1%E0%B8%99%E0%B8%84%E0%B8%A3%E0%B8%B1%E0%B8%9A


