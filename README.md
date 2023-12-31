# waqas_assign1_part3
# Step 1: Created a volume "my_volume"
```
docker volume create my_volume
```
![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/3b69ac48-0af4-416c-8b01-a3df4fdaa767)

# Step 2:
```
docker run -v my_volume:/usr/share/nginx/html -p 8080:80 nginx
```

![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/1ebdc36f-9812-47b1-bb58-8ee46d528ab9)

# Step 3: Verify that the "nginx" default page is accessible on your host machine at http://localhost:8080

![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/10370b23-fcc6-403b-8f93-57cbddd35079)


# Step 4: Created a new file named "index.html" and added some text to it.

# Step 5: Copied the "index.html" file from host machine to the "my_volume" volume using the "docker cp" command.

![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/bf40faf6-3d00-417a-97c3-7e913ec1002e)

# Step 6: Verify that the "index.html" file is accessible on your host machine at http://localhost:8080. (2 marks)

![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/0c33065e-e124-4347-ba37-f3a4f6ace4fe)

# Step 7: Stop and remove the container
```
docker stop awesome_cartwright
```
![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/479a0b56-e026-481f-aacb-19e3f40fe9ad)

```
docker rm awesome_cartwright
```
![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/93723ddf-fcad-467c-9f97-49e80f51432a)

# Step 8: Created a new Docker container using the "httpd" image and mount the "my_volume" volume to it at "/usr/local/apache2/htdocs"
```
docker run -v my_volume:/usr/local/apache2/htdocs -p 8081:80 httpd
```
![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/f8a504cb-3833-41c8-9328-385d1cee3af1)
 
# Step 9: "httpd" default page is accessible on http://localhost:8081

![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/b6e06206-a8d0-4a9f-97d9-f9873ca4896a)


![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/222f006a-ba62-4f4b-a771-4bc15b2303fc)

Step 10: Created a new file named "about.html"
Step 11: Copy the "about.html" file from host machine to the "my_volume"
```
docker cp about.html reverent_blackwell:/usr/local/apache2/htdocs 
```

![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/28ddaa2f-e8dd-484a-8771-ba13768e44ea)

#Step 12: Verify that the "about.html" file is accessible on your host machine at http://localhost:8081/about.html

![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/814f21bb-231e-4680-bd47-eb0ffa80c506)

# Step 13: Stop and remove the container
```
docker stop reverent_blackwell
```
![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/fa8a88ec-b77b-444d-9a72-c864b5de3ed5)

```
docker rm reverent_blackwell
```

![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/1991a15a-6078-4b01-bc90-3ac51e792bff)

# step 14 Verify that the "index.html" and "about.html" files are still available in the "my_volume"
Done

![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/6669ef90-c51f-492b-ac36-a4b3d609af52)

# Step 15 Cleanup: Remove the "my_volume" volume. (2 marks)
```
docker volume rm my_volume
```
![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/17f6f1c7-a1e6-4839-a421-70e949ee25a2)

![image](https://github.com/mwaqaskh/waqas_assign1_part3/assets/39801941/9df615af-115d-4f69-b5ce-c8b2825a992b)

# step 16 Create a README.md file 
Done
