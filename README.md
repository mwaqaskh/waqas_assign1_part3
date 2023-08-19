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
```
docker rm awesome_cartwright
```
