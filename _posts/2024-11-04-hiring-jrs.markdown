---
layout: post
title: "Hiring juniors - devs and cloud"
date: 2021-05-08 08:05:33
categories: hiring
---

Hi! I'm hiring juniors or trainees for development and cloud infra positions.

In the first stage, good candidates will be hired for small, freelance projects. If everything goes fine, this could be a full time job.

I'm working in 3 startups in different fields: cybersecurty, foodtech and hospitality tech.

I defined the job positions as follows:

* BackEnd (Typescript or Python)
* FrontEnd (Typescript)
* FullStack (Typescript or Python)
* Cloud Infra (AWS, Terraform)
* FullStack+Infra (TypeScript, Python, AWS, Terraform)

Feel free to apply to the one you consider the best fit for you.

In the application form, I request a link to a github repo to see the results of the following technical challenges:

# General requirements for the challenge

1. Create an emptoy Github repo.
2. Do not push anything to the main branch.
3. Create a PR with all the code (do not merge it, keep it open for my review).
4. Using AI to accelerate coding is fine.
5. Record a code walkthrough and a demo of your application and paste the link to the video in the PR description. 5 min max.


# Challenge for Backend engineers

## Objective

Create a simple API for managing orders. The API should allow basic CRUD operations and support pagination.

## Requirements
1. **Endpoints**
   - `POST /orders` – Create a new order.
   - `GET /orders/{id}` – Retrieve order details by ID.
   - `PUT /orders/{id}` – Update an order.
   - `DELETE /orders/{id}` – Delete an order.
   - `GET /orders` – Retrieve a list of orders with pagination (`page` and `page_size` parameters).

2. **Order Structure**
   Each order should have:
   - `id` (UUID)
   - `customer_name` (String)
   - `item` (String)
   - `quantity` (Integer)
   - `status` (Enum: `pending`, `completed`, `cancelled`)
   - `created_at` (Timestamp)

3. **Pagination**
   Support pagination for `GET /orders` with `page` and `page_size` parameters.

4. **Bonus**
   - Filtering by `status` in `GET /orders`.
   - Add a README with setup instructions.
   - Unit tests.

# Challenge for FrontEnd Engineers

## Objective
Build a simple frontend interface for managing orders. The application should display a list of orders, support basic CRUD operations, and implement pagination.

## Requirements
1. **Order List View**
   - Display a list of orders with the following fields:
     - `Order ID`
     - `Customer Name`
     - `Item`
     - `Quantity`
     - `Status` (e.g., `pending`, `completed`, `cancelled`)
   - Paginate the order list with `Next` and `Previous` buttons.

2. **Order Details**
   - Allow users to view more details of a selected order.

3. **Create/Edit Order**
   - Provide a form to create a new order or edit an existing order with fields:
     - `Customer Name` (input)
     - `Item` (input)
     - `Quantity` (input)
     - `Status` (dropdown with options: `pending`, `completed`, `cancelled`)

4. **Delete Order**
   - Allow users to delete an order from the list.

5. **Data Handling**
   - Use a mock API (e.g., JSON server or in-memory mock) for data retrieval and manipulation.
   - Handle API responses, loading states, and error states.

6. **Bonus**
   - Filter the order list by `Status`.
   - Add a README with setup instructions.
   - Include basic unit tests for components.

# Coding for FullStack Engineers

## Objective
Build a simple Order Management System with both frontend and backend components. The backend should handle CRUD operations and support pagination, while the frontend should allow users to interact with the order data seamlessly.

## Requirements

### Backend
1. **API Endpoints**
   - `POST /orders` – Create a new order.
   - `GET /orders/{id}` – Retrieve order details by ID.
   - `PUT /orders/{id}` – Update an order.
   - `DELETE /orders/{id}` – Delete an order.
   - `GET /orders` – Retrieve a paginated list of orders (`page` and `page_size` parameters).

2. **Order Structure**
   Each order should contain:
   - `id` (UUID)
   - `customer_name` (String)
   - `item` (String)
   - `quantity` (Integer)
   - `status` (Enum: `pending`, `completed`, `cancelled`)
   - `created_at` (Timestamp)

3. **Pagination**
   Support pagination for `GET /orders`.

### Frontend
1. **Order List View**
   - Display a paginated list of orders with the following fields:
     - `Order ID`
     - `Customer Name`
     - `Item`
     - `Quantity`
     - `Status`
   - Implement `Next` and `Previous` buttons for pagination.

2. **Order Details**
   - Allow users to click on an order to view more details.

3. **Create/Edit Order**
   - Provide a form to create a new order or edit an existing order with fields:
     - `Customer Name` (input)
     - `Item` (input)
     - `Quantity` (input)
     - `Status` (dropdown with options: `pending`, `completed`, `cancelled`)

4. **Delete Order**
   - Allow users to delete an order from the list.

5. **Error and Loading States**
   - Handle API responses, including loading and error states.

### Bonus
- **Backend**: Add filtering by `status` for `GET /orders`.
- **Frontend**: Add a filter option to view orders by `status`.
- **Testing**: Include basic unit tests for both frontend components and backend endpoints.
- **Documentation**: Add a README with setup instructions for both frontend and backend.


# Challenge for Cloud Engineers

## Objective
Build an infrastructure setup on AWS to deploy a scalable web application using **Terraform**, **ECS**, and **AWS networking best practices**.

## Requirements

1. **Infrastructure with Terraform**
   - Use **Terraform** to create a **modular** setup.
   - Implement remote state with S3 and DynamoDB for state locking.

2. **ECS and Load Balancing**
   - Deploy a containerized web app (e.g., NGINX) on **ECS Fargate**.
   - Configure **auto-scaling** for the ECS tasks (min 1, max 3).
   - Use an **Application Load Balancer** (ALB) for traffic distribution.

3. **Networking and Security**
   - Set up a **VPC** with public/private subnets across multiple AZs.
   - Use **security groups** to allow only HTTP/HTTPS traffic from the ALB.
   - Configure IAM roles for ECS tasks with **least privilege** permissions.

4. **Optional (Bonus): Monitoring and Alarms**
   - Set up basic **CloudWatch alarms** for ECS (e.g., CPU and memory).


# Challenge for FullStack + Infra engineers

If you are interested in applying for FullStack with Cloud Infra skills, feel free to mix both challenges in a single PR :)

# How to apply

Apply here: https://airtable.com/appUkxpvzu2PeWYer/pagqD1NOksubT0Z96/form

 
