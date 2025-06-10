### Tested: ok (in RPi3b+)

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).



## Getting Started


Install the dependencies: (listed in package.json file)

```bash
npm install
# or
npm i
```


Run the development server:

```bash
npm run dev ✓
# or
yarn dev
# or
pnpm dev
```



Open [http://localhost:3000](http://localhost:3000) or [http://host_ip:3000](http://rpi_ip:3000) with your browser to see the result.

You can start editing the Home page by modifying

```bash
app/page.js
```

The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
   

## Ho to run this app using docker-compose

```bash
$ sudo docker-compose up -d
$ sudo docker ps

if application is running without Nginx  
proxy server, then..  
Open  
http://localhost:3000  (or)    
http://host-ip:3000   
with your browser to see the result. 
    
     
if application is running with Nginx  
proxy server, then..  
Open  
http://localhost   (or)     
http://host-ip
```

## How to enter into the running container 

```bash
$ sudo docker ps
$ sudo docker logs container-name
$ sudo docker exec -it container-name sh
$ ls -la
```

## How to remove the app

```bash
$ sudo docker-compose down
$ sudo docker ps
$ sudo docker system prune -a

$ cd ..
$ ls -l
$ sudo rm -r docker-nextjs-boilerplate-app/
$ ls -l
```