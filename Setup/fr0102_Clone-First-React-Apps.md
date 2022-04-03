
<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Test NodeJS](/Setup/fr0102_Test-Node.md)
</div><div class="page-next">

[Vultr Ubuntu - NEXT](/Setup/fr0301_Setup-Vultr-Ubuntu.md)
</div><div style="margin-top:35px">&nbsp;</div> 
 
<!-- ------------------------------------------------------------------------- -->

## 1.3 Clone First React Apps 0:45
- [Purpose and Background](../Setup/purposes/pfr0102_Clone-First-React-Apps.md)
- [Enter Comments in Discord](https://discord.com/channels/928752444316483585/931216956827250709)

#### Introduction  
- First React Apps is a collection of applications that use React. The apps increase from simple through database access. For the rest of the tutorial we will focus on React apps. 
- In this topic you will clone and test these basic React applications on your local workstation.


#### Important note about names, capitalization, pictures and code copying
- In this tutorial please be careful to use the Exact Spelling and Capitalization. You will be using Windows, Unix and GitBash command prompts. Improper captialization will cause commands to fail. Some examples are: Local_Admin, myProject, repos, remotes and .ssh.
- This documentation was produced in 2021-2022. You will experience differences in some of the pictures due to the changes made over time by the developers of the softwares and web sites that are used.
- We recommend that you cut and paste code snippets from the Documentation into your workstation/server. This will reduce the errors caused by hand typing.


----


### 1 Clone FRApps Repository 0:05
----
1. Clone into the local repos folder using the Windows Command prompt

```
cd C:\repos\
```
 
![FRApps-Clone-01](images/fr0103-FRApps-Clone-01.png "FRApps-Clone-01")

 
```
git clone https://github.com/8020data/FRApps_prod-master.git FRApps

cd FRApps

dir
```

![FRApps-Clone-02](images/fr0103-FRApps-Clone-02.png "FRApps-Clone-02")

2. Enter the following in the terminal. (It will open VSCode)

```
code FRApps.code-workspace
```

- If prompted, click "Yes I trust the authors".

![FRApps-Clone-03](images/fr0103-FRApps-Clone-03.png "FRApps-Clone-03")
 
----
### 2. Install Node modules  0:15
----
1. Right click on the client folder

2. Click Open in Integrated Terminal, then 

![FRApps-Clone-04](images/fr0103-FRApps-Clone-04.png "FRApps-Clone-04")

```
npm install
```

![FRApps-Clone-05](images/fr0103-FRApps-Clone-05.png "FRApps-Clone-05")

3. Test for production vulnerabilities

```
npm audit --production
```

![FRApps-Clone-06](images/fr0103-FRApps-Clone-06b.png "FRApps-Clone-06")

4. Right click on the server folder

5. Click Open in Integrated Terminal, then 

![FRApps-Clone-07](images/fr0103-FRApps-Clone-07.png "FRApps-Clone-07")

```
npm install 
```

![FRApps-Clone-08](images/fr0103-FRApps-Clone-08.png "FRApps-Clone-08")

![FRApps-Clone-09](images/fr0103-FRApps-Clone-09.png "FRApps-Clone-09")

----
 ### 3. Run Client 1c-react-empty application 0:05
----

1. Right click on the client/1c-react-empty folder
2. Click Open in Integrated Terminal, then 

![FRApps-Clone-21](images/fr0103-FRApps-Clone-21.png "FRApps-Clone-21") 

```
npm start
```

![FRApps-Clone22](images/fr0103-FRApps-Clone-22.png "FRApps-Clone-22")

- If you are prompted, click Allow Access

![FRApps-Clone22a](images/fr0103-FRApps-Clone-22a.png "FRApps-Clone-22a")

![FRApps-Clone22b](images/fr0103-FRApps-Clone-22d.png "FRApps-Clone-22b")

![FRApps-Clone22b](images/fr0103-FRApps-Clone-22b.png "FRApps-Clone-22b")


----
 ### 4. Run Client 2c-react-button application 0:05
----

1. Right click on the client/2c-react-button folder
2. Click Open in Integrated Terminal, then 

![FRApps-Clone-31](images/fr0103-FRApps-Clone-31.png "FRApps-Clone-31") 

```
npm start
```

![FRApps-Clone33](images/fr0103-FRApps-Clone-33.png "FRApps-Clone-33")

![FRApps-Clone33a](images/fr0103-FRApps-Clone-33a.png "FRApps-Clone-33a")

- Click the Like button.

![FRApps-Clone33b](images/fr0103-FRApps-Clone-33b.png "FRApps-Clone-33b")

----
 ### 5. Run Client 3c-react-no-api application 0:05
----

1. Right click on the client/3c-react-no-api folder
2. Click Open in Integrated Terminal, then 

![FRApps-Clone-41](images/fr0103-FRApps-Clone-41a.png "FRApps-Clone-41") 

```
npm start
```
![FRApps-Clone-41](images/fr0103-FRApps-Clone-41.png "FRApps-Clone-41") 

![FRApps-Clone44](images/fr0103-FRApps-Clone-44.png "FRApps-Clone-44")

![FRApps-Clone44a](images/fr0103-FRApps-Clone-44a.png "FRApps-Clone-44a")

3. Click Invoices, then Santa Monica

![FRApps-Clone44b](images/fr0103-FRApps-Clone-44b.png "FRApps-Clone-44b")

----
 ### 6a. Run Server 4s-react-wi-api application 0:05
----

1. Right click on the server/4s-react-wi-api folder (Note: server folder not client)
2. Click Open in Integrated Terminal, then 

![FRApps-Clone-51](images/fr0103-FRApps-Clone-51.png "FRApps-Clone-51") 

```
npm start
```

![FRApps-Clone55](images/fr0103-FRApps-Clone-55.png "FRApps-Clone-55")

![FRApps-Clone55a](images/fr0103-FRApps-Clone-55a.png "FRApps-Clone-55a")

3. Browse to

```
http://localhost:50114/invoices
```

![FRApps-Clone55b](images/fr0103-FRApps-Clone-55b.png "FRApps-Clone-55b")

#### Note: Keep this step 6a running when you do step 6b (next step)

----
 ### 6b. Run Client 4c-react-wi-api application 0:05
----

#### Note: Be sure step 6a is running
<br/>

1. Right click on the client/4c-react-wi-api folder (note: client folder not server)
2. Click Open in Integrated Terminal, then 

![FRApps-Clone-61](images/fr0103-FRApps-Clone-61.png "FRApps-Clone-61") 

```
npm start
```

![FRApps-Clone66](images/fr0103-FRApps-Clone-66.png "FRApps-Clone-66")

![FRApps-Clone66a](images/fr0103-FRApps-Clone-66a.png "FRApps-Clone-66a")

![FRApps-Clone-66b](images/fr0103-FRApps-Clone-66b.png "FRApps-Clone-66b")

3. Click Invoices, then Ocean Avenue

![FRApps-Clone-66c](images/fr0103-FRApps-Clone-66c.png "FRApps-Clone-66c")

----
 ### 7. Run Client 5c-my-react-app application 0:05
----

Note: This app is based on this [W3C Tutorial](https://www.w3.org/Style/Examples/011/firstcss.en.html)
<br></br>

1. Right click on the client/5c-my-react-app folder
2. Click Open in Integrated Terminal, then 

![FRApps-Clone-67](images/fr0103-FRApps-Clone-67.png "FRApps-Clone-67") 

```
npm start
```

![FRApps-Clone68](images/fr0103-FRApps-Clone-68.png "FRApps-Clone-68")

- If you are prompted, click Allow Access

![FRApps-Clone68a](images/fr0103-FRApps-Clone-22a.png "FRApps-Clone-68a")

![FRApps-Clone68d](images/fr0103-FRApps-Clone-68d.png "FRApps-Clone-68d")

![FRApps-Clone68b](images/fr0103-FRApps-Clone-68b.png "FRApps-Clone-68b")


----
#### Congratulations! You have cloned and run the FRApps successfully to your local workstation.
----

<!-- ------------------------------------------------------------------------- -->

<div class="page-back">

[BACK - Test NodeJS](/Setup/fr0106_Test-Node.md)
</div><div class="page-next">


[Vultr Ubuntu - NEXT](/Setup/fr0301_Setup-Vultr-Ubuntu.md)
</div>

<!-- ------------------------------------------------------------------------- -->