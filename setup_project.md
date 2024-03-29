# Setup Project  

### 1. Install Vue CLI

ดู npm (node package manager) version ในเครื่อง
```sh
$ npm --version
6.11.3
```
ติดตั้ง @vue/cli
```sh
$ npm install -g @vue/cli
```
ดู vue version
```sh
$ vue --version
@vue/cli 4.1.1  
```
### 2. Create Project

```sh
$ vue create <PROJECT_NAME> 
```
? Please pick a preset : เลือกเป็น default  

![](create-project_1.png)

? Pick the Package Manager : เลือกเป็น YARN 

![](create-project_2.png)

### 3. Run Dev  

```sh
$ cd <PROJECT_NAME>  
$ yarn serve 
```

ลองเข้า http://localhost:8080/    

# Project Structure  

<img src="project-structure.png" width="400px"/>

# Build for Production 

```sh
$ yarn build 
```

มันจะสร้าง folder `dist` ซึ่งเป็น folder ที่มีการ compile และบีบอัด code ส่วนต่าง ๆ เพื่อนำไป run บน production  

# Run Dist 

### 1. Install Serve  
```sh
$ npm install -g serve  
$ serve --version  
11.2.0  
```

### 2. Run 
```sh
$ serve -s dist  
```

ลองเข้า http://localhost:5000 

### 3. เปลี่ยน port 
```sh
$ serve -s dist -l 8080  
```

ลองเข้า http://localhost:8080   
