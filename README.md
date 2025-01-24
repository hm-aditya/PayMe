- Clone the repo

```jsx
git clone https://github.com/hm-aditya/PayMe.git

- npm install
- Run postgres either locally or on the cloud (neon.tech)

```jsx
docker run  -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres
```

- Copy over all .env.example files to .env
- Update .env files everywhere with the right db url
- Go to `packages/db`
    - npx prisma migrate dev
    - npx prisma db seed
- Go to `apps/user-app` , run `npm run dev`
- Try logging in using phone - 1111111111 , password - alice (See `seed.ts`)
- Go to `apps/bank-webhook`,run `npm run dev` or  run `node dist/index.js`

 ## Transfer page
 ![Screenshot 2025-01-24 122053](https://github.com/user-attachments/assets/6723a8f7-ccbb-430b-bfdb-2b63061d84ac)

## Redirected to Bank page
 ![Screenshot 2025-01-24 122110](https://github.com/user-attachments/assets/8a1b5933-e8bf-4978-95ac-ea3de0831d8f)

## the transfer data in database
![Screenshot 2025-01-24 122139](https://github.com/user-attachments/assets/c938951f-4d8c-4b13-8a7b-f2fde58a0987)

## on ramp transaction done by sending post request through postman with content like token_id,amount,user_id
![Screenshot 2025-01-24 122230](https://github.com/user-attachments/assets/135c9bd7-7b41-4b39-a883-6e0f1d0ba72c)

## transaction successfull 
 ![Screenshot 2025-01-24 122243](https://github.com/user-attachments/assets/ac24def3-e254-4343-bc3c-a21231c105b4)

## transaction reflected on user1 dashboard/frontend
![Screenshot 2025-01-24 122257](https://github.com/user-attachments/assets/6752aedd-e430-4606-8e8b-0c49c83ac631)

## Transactions log page
![Screenshot 2025-01-24 122313](https://github.com/user-attachments/assets/69b297df-2b29-42ee-9d06-8077d19719fd)

## p2p transfer to user2 (bob with phone-no 2222222222)
![Screenshot 2025-01-24 122412](https://github.com/user-attachments/assets/6c1392d9-4575-4436-82e3-c76d05d9091e)

## user2 initial balance
![Screenshot 2025-01-24 122509](https://github.com/user-attachments/assets/2a17f1c8-1c9c-49da-a9f5-af9466478109)

## user2 balance after transaction / getting 1000 INR from user1 (1111111111 /alice )
![Screenshot 2025-01-24 124114](https://github.com/user-attachments/assets/f85f65a9-5ced-4be7-b69f-1fb0ecc49e21)
 






  
