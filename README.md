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

[คำแนะนำจาก git ช่วยได้เยอะ](https://github.com/suntana-kmitl/6004c/blob/main/git_config1.png)

สังเกตว่า git ตั้งชื่อ branch ว่า  main  ให้เรา

5. sync folder ของเราไปที่ main
สั่ง
<!-- Code Blocks -->
```git
git push -u origin main 
```
login เข้า git ตามที่ คำสั่ง push แนะนำ

[ตัวอย่างการสั่งงาน](blob/main/git_scenario1_try1.png)

ทุกครั้งก่อนที่จะ push ใหม่ ก็ commit -am "[memo to this commit]"  

git จะทำทุกอย่างที่เราทำกับไฟล์ที่มัน track อยู่ ดังนั้น ตอนนี้ควรลบ แฟ้ม .git ทิ้งไปก่อน 

เมื่อเราเชี่ยวชาญกว่านี้เราค่อยปล่อยให้มันทำงาน

---

[^1]: คำสั่งครั้งเดียวเพื่อ ตั้งค่า configuration ของ git account จาก client คือ

<!-- Code Blocks -->
```git
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

[git_config1.png](git_config1.png)

location ของไฟล์นี้ จะหาให้ดูโอกาสต่อๆไป