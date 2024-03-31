# PIA STORE WEB APPLICATION

<div align="center">
  <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/3a1bc3c3-c144-47fb-a1f6-47e39669617d" width="60%"/>
  <h2 align=center>This repository contains three submodules of the project which is a pia store web application using MERN Stack 
    <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/e8a26f98-0921-4122-a4d5-e661b4b766d0" width="5%" /> 
  </h2>
</div>
<div>
  <b>Pia store web application</b> has been built and developed so as to manage the purchase and sale activities for Banh Pia, which is one of the most famous traditional cakes in Viet Nam. </br></br>
  In this project, I decided to obtain and analyze the e-commerce process. And afterwards, I commenced creating the pia store website system 
  which consists of sufficient basic functions of an e-commerce website system, such as reviewing products, adding products to cart, checking out and ordering, managing order history,... 
  Moreover, I also built a website management for the storekeeper in order to manage all products, all orders,... 
</div>
</br></br>

> **Three submodules of this project includes:**<br/>
> i) A front-end for customers which allows them to review and purchase products.<br/>
> ii) A front-end for administrators which allows them to manage the purchase and sale activities of the system.<br/>
> iii) A back-end.<br/></br>

---

## Documentation
### Project Structure 
</br>
<div align="center">
  <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/aca5be88-4dae-49d1-b610-c1f91dd14eb7" width="70%"/>
</div>

### CDM
</br>
<div align="center">
  <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/81e210d0-b3b4-4dee-a8fc-3ba891311d0e" width="70%"/>
</div>

### Project Figures
<details open>
  </br>
  <summary><b>Customer Side</b></summary>

  <div align="center">
    <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/44215b74-b776-4991-970a-d578bfc8f27a" width="70%"/>
    <div>
      <em><b>Figure 1.</b> Home page</em>
    </div>
  </div>
  </br>
  
  <div align="center">
    <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/b9d9b6f1-8a87-4863-b49d-2fc9ac8cda87" width="70%"/>
    <div>
      <em><b>Figure 2.</b> Product detail page</em>
    </div>
  </div>
  </br>

  <div align="center">
    <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/d528127f-86cf-4110-b6d9-16861a2b8c68" width="70%"/>
    <div>
      <em><b>Figure 3.</b> Cart page</em>
    </div>
  </div>
  </br>

  <div align="center">
    <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/7c5e54b0-e466-471e-99bc-bbd9f009f933" width="70%"/>
    <div>
      <em><b>Figure 4.</b> Order history page</em>
    </div>
  </div>
  </br>

  <div align="center">
    <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/6c83458a-7c3e-4153-8127-6406ce5074dd" width="70%"/>
    <div>
      <em><b>Figure 5.</b> Review page</em>
    </div>
  </div>
  </br>
</details>

<details open>
  </br>
  <summary><b>Admin Side</b></summary>

  <div align="center">
    <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/b7475288-83c4-48ef-ab57-71daa9a0571a" width="70%"/>
    <div>
      <em><b>Figure 6.</b> Product management page</em>
    </div>
  </div>
  </br>

  <div align="center">
    <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/a9093b74-af54-44f1-acab-30dad8cd9c92" width="70%"/>
    <div>
      <em><b>Figure 7.</b> Order management page</em>
    </div>
  </div>
  </br>

  <div align="center">
    <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/cf9a0d85-e75c-4e24-93ff-7e774dc5d106" width="70%"/>
    <div>
      <em><b>Figure 8.</b> Order detail modal popup</em>
    </div>
  </div>
  </br>
</details>


### Members
<table>
  <tr>
    <td align="center">
        <a href="https://github.com/HoTranThienNhan">
            <img src="https://github.com/HoTranThienNhan/PiaStoreWebApp/assets/122293496/a0fefa28-d860-49bb-907d-59d8ebaf4a04" width="100px;" alt=""/>
            <br /><sub><b>Thien Nhan</b></sub>
          </a>
        </a>
      </td>
  </tr>
</table>

---

## Setup And Usage
### Installation and setup 
```bash
### Cloning this repository:
$ git clone --recurse-submodules https://github.com/HoTranThienNhan/PiaStoreWebApp.git
$ cd PiaStoreWebApp

### Installing all dependencies of each submodule:
# pia-store-customer:
$ cd pia-store-customer
$ npm install

# pia-store-admin:
$ cd pia-store-admin
$ npm install

# pia-store-server:
$ cd pia-store-server
$ npm install
```

### Database
``` bash
### In MongoDB Compass (localhost: 27017) shell, preparing for database and its collections:
# creating 'piastore' database if not exists
> use piastore

# creating 4 collections: products, users, orders, reviews
> db.createCollection("products")
> db.createCollection("users")
> db.createCollection("orders")
> db.createCollection("reviews")
```
To access admin website system, importing [this json file](https://github.com/HoTranThienNhan/PiaStoreWebApp/files/14533120/admin-piastore-account.json) to <em>'users'</em> collection of <em>'piastore'</em> database which has already created:

```
{
  "_id": {
    "$oid": "650a5486f01b355bfdc497c6"
  },
  "fullname": "admin",
  "email": "admin@gmail.com",
  "password": "$2b$10$M/mQhDxPs0P1v8BK7Anvu.uyO.Oermi66g.h6nCwKWBby3pqkBpB2",
  "isAdmin": true,
  "phone": "0987654321",
  "createdAt": {
    "$date": "2023-09-20T02:10:14.439Z"
  },
  "updatedAt": {
    "$date": "2023-11-23T03:35:32.500Z"
  },
  "__v": 0,
  "address": "Your Address",
  "avatar": "",
  "active": true
}
```
<details>
  <summary><b>Testing admin account infomation (for accessing admin web), click to show details</b></summary>
  <div>
    <b>Email:</b> admin@gmail.com
  </div>
  <div>
    <b>Password:</b> admin123
  </div>
  
</details>

### Run
``` bash
### Running each submodule:
# pia-store-customer (running on localhost:3000):
$ cd pia-store-customer
$ npm start

# pia-store-admin (running on localhost:3002):
$ cd pia-store-admin
$ npm start

# pia-store-server (running on port 3001):
$ cd pia-store-server
$ npm start
```

---

## DEPLOYMENT
### This e-commerce website's React.Js module has been deploying with <a href="https://vercel.com/">Vercel</a> and Node.js module with <a href="https://render.com/">Render</a>. 

Link to preview here: https://pia-store-customer.vercel.app/
