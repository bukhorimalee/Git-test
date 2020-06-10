(feature-2)
# Git-test-codecamp-6
## markdown
# title h1
## title h2
### title h3
#### title h4
##### titlte h6
*This is Codecamp*
**This is Codecamp**
*__This is Codecamp__*
>สร้าง blockquotes >
>> ไห้ใช้คำสั่งมากกว่า >>
>>> ไห้ใช้คำสั่งมากกว่า >>
> test
>> test 	
> Quoted text.
> > Quoted quote.
> * Quoted 
> * List 
> - This Is List 1
> - This Is List 2
> - This Is List 3
> + This is order 1
> + This is order 3

    * this is facebook
    ![detail pic] (url) = picture
***, ---, ______ = <hr>
![content](https://scontent.fbkk5-4.fna.fbcdn.net/v/t1.0-9/p960x960/96016427_1155406918128901_2059772135118733312_o.jpg?_nc_cat=110&_nc_sid=85a577&_nc_eui2=AeGx8pBt6lY7uLt9nBCd_U2xzoP7_YdnxKDOg_v9h2fEoGsyg5aF4hd_aF0uzktbQxG4jYb1Cr2hbbC9VMh8HnFe&_nc_oc=AQmOh6paylDfLGz686OUeeRB5VaShe9JrAwe8qz6WprkPCi57zrpOSEc6lIExkLFsRfLLsmqje-2UIzTVrb4Y2ai&_nc_ht=scontent.fbkk5-4.fna&_nc_tp=6&oh=33efa3ddb2d16852aedb90423562afd0&oe=5EFE0A55) [Click Here](https://www.facebook.com/bukhori.malee.9) Facebook Here
      
               fdgdssaer
            **This is Codecamp**  
            
<hr>  

  
   
When `x = 3`, inline code ก็คิอ แทืก < code > ของ htmlนั่นเอง `x + 2 = 5`

# git flow
- edid file
- git add
- git commit -m "title"-m "description เก็บข้อมูลขึ้น remote repro
- git push หากต้องการเอาขึ้น remote repro
- git pull ดึงข้อม฿ลจาก remote repro, dowload file
![content](https://3.bp.blogspot.com/-Wdqrzw1boBw/WbbHN3XFETI/AAAAAAAACV4/2r6we5RxnIMzXavPDr3FZvbM1sgZUrdBQCLcBGAs/s1600/git_138.jpg)
![git graph master](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTNLeFI8crFRcYUvqT47I-ky1yn0dY5xSvE30Bwe8XAkZ_S0Gdn&usqp=CAU)# การแตก Respository
## Git
- git add .
git commit -m "first commit"
git push -u origin master `ส่งไฟล์`
- git restore . `ดึงไฟล์กลับมา`
## Git Branch : เพิ่ม ลบ แสดงกิ่งของ Repository
- git branch
- git branch --all          `เช็ค กิ่ง repository`
- git branch --list `เช็คว่ามี branch อะไรบ้าง
- git branch develop        `สร้าง branch ชื่อ develop`
- git branch --delete develop , git branch -d develop `ลบ branch ชื่อ develop`
- git checkout <branch name, commot id>  `ย้ายการทำงานไปที่ Branch หรือ commit id ที่ระบุ`
- git checkout -b test `สร้าง branch ชื่อ test และทำการสลับการทำงานมาที่ branch นี้ ก็ือ test นั้นเอง`
- git checkout <branch name> <file name>    `เลือกแค่บางไฟล์จาก Branch อื่น เข้ามา Merge กับ Working Directory ที่กำลังทำการ`
- git push --set-upstream origin develop `git ขึ้น Branch บนฐ้านข้อมูล
<<<<<<< HEAD
- git push -u origin develop `ขึ้น ไฟล์ Branch Develop บนฐ้านข้อมูล
## Git merge 
- เป็นการรวมข้อมูล จาก branch ไป อีก branch เช่น เราต้องการ นำข้อมูลจาก develop ไปรวมกับ master
=======
- git push -u origin develop `ขึ้น ไฟล์ Branch Develop บนฐ้านข้อมูล
- git merge ชื่อ branch ที่จะเอาไว้รวม กับbranchที่เลือกไว้ในปัจจุบัน
- git log --oneline --decorate --graph --all `ดู merge ทั้งหมด `

# Git command Trict
- git commit -am ".."  `เพื่อที่จะ git add พร้อม git commit`
- git commit -am “title” -m “description”
- git checkout -b name- 
- git branch -m old_name new_name `เปลียนชื่อเก่า ใหม่ `
- git log --oneline --decorate --graph --all `ดู แผงผัง Branch `
- git merge branch_name -m “description” ` การ Merge และ commit พร้อมกัน `
- git merge branch_name --no--ff (no fast forward) ` เปิดปิด Merge `
# Git Rebase
rebase เป็นการย้ายข้อมูล จาก branch หนึ่งมาต่ออีก branch 
 ขั้นตอนการทำ rebase จาก dev to master
1. update repo
2. checkout master
3. git pull
4. git rebase dev
6. ตรวจสอบ conflict
7. ถ้ามีให้แก้ไข save แล้ว git add
8. ถ้าไม่มีให้ git add ได้เลย
9. git rebase --continue
10. git commit and push
- git rebase develop develop เอาข้อมูลจาก develop เข้าไปใน merge ที่เลือกในปัจจุบัน