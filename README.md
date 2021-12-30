git hub ฉบับย่อมาก

scenario 1 สร้าง git เป็น backup

หลังจากติดตั้ง git แล้ว[^1] ใน folder ที่ต้องการ 
1. สั่ง

<!-- Code Blocks -->
```git
git init
```

2. สั่ง
<!-- Code Blocks -->
```git
git add .
```
เพื่อ ให้ทุกไฟล์ใน folder นี้อยู่ในสถานะ **staged**

3. สั่ง 
<!-- Code Blocks -->
```git
git commit -am "memo to this commit"
```
เพื่อให้เป็นจุดบันทึกสถานะของไฟล์สำหรับการ push

4. ไปสร้าง repo ที่ github แล้ว จำ path ของ repo ไว้

สั่ง git remote add origin [https://github.com/[user]/[reponame]]()

[คำแนะนำจาก git ช่วยได้เยอะ](git_scenario1.png)

สังเกตว่า git ตั้งชื่อ branch ว่า  main  ให้เรา

5. sync folder ของเราไปที่ main
สั่ง
<!-- Code Blocks -->
```git
git push -u origin main 
```
---

[^1]: คำสั่งครั้งเดียวเพื่อ ตั้งค่า configuration ของ git account จาก client คือ

<!-- Code Blocks -->
```git
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

[git_config1.png](git_config1.png)

location ของไฟล์นี้ จะหาให้ดูโอกาสต่อๆไป