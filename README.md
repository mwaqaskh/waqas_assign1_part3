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
