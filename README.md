# Git

## Add git	- เพิ่ม git ใน Folder นั้นๆ
  
  Command :
  
    git init
  
  Example :
  
    C: ..\Path\projectCode git init
  				
  
## Add File - เพิ่มไฟล์   
  ### Command เพิ่มบางไฟล์ :
  
    git add <fileName.typeFile>		
    
   Example :   
  
    git add README.md			    
    
  ### Command เพิ่มไฟล์ทั้งหมด
  ##### ที่อยู่ในโฟลเดอร์หรือ Path นั้น :

    git add .				
    	
## Commit File 
  Command & Example : 
  
    git commit -m "message commit"
  
					
## Add Branch - เพิ่ม Branch		
  Command & Example : 
  
    git branch -M main			
    
## Add URL Remote Server - เพิ่ม url ของ Remote (Server) เพื่อให้รู้ว่าเราจะฝากโค้ดไว้ที่ใด		
  Command & Example : 
  
    git remote add origin https://github.com/Siraswaya/learning.git				
    
## Push Code to Server - ส่งโค้ดไปที่ Github Server
  Command & Example : 
  
    git push -u origin main	
    
  - u : เอาไว้จำ parameter origin master ต่อไปก็แค่พิมพ์ git push			
  - origin : คือชื่อ alias ของ remote (github)			
  - master : คือชื่อ branch ที่เราต้องการ push ขึ้นไป									
						
## Create New Branch - สร้าง Branch ใหม่		
  Command & Example : 
  
    git branch branchNameNew		
    
## Change Other Branch - เปลียนไปใช้ Branch	อื่น
Command & Example : 

    git checkout branchName				
    
## Fetch ข้อมูลระหว่าง Local กับ Github (remote) ว่ามีโค้ดส่วนใดต่างกัน		
Command & Example : 

    git fetch				
    
## Git Pull รวมโค้ดจาก Github (remote) มาที่เครื่อง Local				
Command & Example : 

    git pull

## Git Merge - ผสาน Branch ที่มีการแก้ไข				
Command & Example : 

    git merge origin/master
    
 > เมื่อ Merge แล้วให้ทำการ Commit โดยใช้คำสั่ง git Commit
    
## Delete - ลบ Branch		
Command & Example : 

    git branch -d branchName	
    
## Remove origin - ลบ origin	
Command & Example : 
    		
    git remote rm origin		
    
## Git Clone - คัดลอกโปรเจ็คนั้นมาไว้ที่เครื่องของเรา    
Command :

    git clone gitURL		
    
Example : 

    git clone https://github.com/Siraswaya/learning.git
						
		
						
