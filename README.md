# Git

## Add git - เพิ่ม git ใน Folder ที่เครื่อง Local ที่ต้องการส่งขึ้น Server
  > โดยเมื่อ Run คำสั่งนี้เสร็จแล้ว จะมีการสร้างไฟล์ .git ขึ้นใน Path 
  Command :
  
    git init
  
  Example :
  
    C: ..\Path\projectCode git init
  
  
  
  
## Add File - เพิ่มไฟล์ที่ต้องการนำขึ้น Server 
> สามารถเพิ่มแค่บางไฟล์ที่ต้องการ หรือจะเพิ่มทั้งหมดก็ได้ โดยจะใช้คำสั่งดังต่อไปนี้

  ### Command เพิ่มบางไฟล์ :
  
    git add <fileName.typeFile>		
    
   Example :   
  
    git add README.md	
    
  ### Command เพิ่มไฟล์ทั้งหมด
  ##### ที่อยู่ในโฟลเดอร์หรือ Path นั้น :

    git add .				
    	
## Commit File 
> เมื่อเรา Commit จะทำให้เราสามารถย้อนมาดูได้ว่ามีการแก้ไขอะไรไปบ้าง

  Command & Example : 
  
    git commit -m "message commit"
    
## Push File 
> เป็นการส่งข้อมูลจาก Local ไปยัง Remote Repository

  Command & Example : 
  
    git push origin master
					
## Add Branch 	
  Command & Example : 
  
    git branch -M main			
    
## Add URL Remote Server
> เพิ่ม url ของ Remote (Server) เพื่อให้รู้ว่าเราจะฝากโค้ดไว้ที่ใด		
  Command & Example : 
  
    git remote add origin https://github.com/Siraswaya/learning.git				
    
## Push Code to Server 
> ส่งโค้ดไปที่ Github Server
  Command & Example : 
  
    git push -u origin main	
    
  - u : เอาไว้จำ parameter origin master ต่อไปก็แค่พิมพ์ git push			
  - origin : คือชื่อ alias ของ remote (github)			
  - master : คือชื่อ branch ที่เราต้องการ push ขึ้นไป									
						
## Create New Branch  
> สร้าง Branch ใหม่		
  Command & Example : 
  
    git branch branchNameNew	
    
> สามารถใช้คำสั่ง git branch เพื่อดูว่าปัจจุบันอยู่ที่ Branch ใดได้

   	git branch
    
## Git Checkout (Switch Other Branch)
> เปลียนหรือสลับไปใช้ Branch อื่น
Command & Example : 

    git checkout branchName				
    
## Git Fetch 
> ข้อมูลระหว่าง Local กับ Github (remote) ว่ามีโค้ดส่วนใดต่างกัน		
Command & Example : 

    git fetch				
    
## Git Pull 
> รวมโค้ดจาก Github (remote) มาที่เครื่อง Local				
Command & Example : 

    git pull

## Git Merge 
> ผสาน Branch ที่มีการแก้ไข				
Command & Example : 

    git merge origin/master
    
 > เมื่อ Merge แล้วให้ทำการ Commit โดยใช้คำสั่ง git Commit
    
## Delete Branch
> ลบ Branch		
Command & Example : 

    git branch -d branchName	
    
## Remove origin 
> ลบ origin	
Command & Example : 
    		
    git remote rm origin		
    
## Git Clone
> คัดลอกโปรเจ็คนั้นมาไว้ที่เครื่องของเรา    
Command :

    git clone gitURL		
    
Example : 

    git clone https://github.com/Siraswaya/learning.git
    
## Git Force Pull 
> รวมโค้ดจาก Github (remote) มาที่เครื่อง Local	โดยจะทำการบังคับดึงข้อมูลมาทับไฟล์ในเครื่อง Local ทั้งหมด			
Command & Example : 

First, run a fetch to update all origin/<branch> refs to latest:

	git fetch --all
	
Backup your current branch:

	git branch backup-master
	
Then, you have two options:

	git reset --hard origin/master
	
OR If you are on some other branch:

	git reset --hard origin/<branch_name>
    
    
    
    
## Ref

https://stackoverflow.com/questions/1125968/how-do-i-force-git-pull-to-overwrite-local-files
						
		
						
