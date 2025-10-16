---
layout: post
title: "Hiring Full Stack Junior Engineers - TypeScript Ecosystem"
date: 2025-10-14 08:05:33
categories: hiring
---

Hi! I'm hiring junior or trainee full stack engineers with experience in the TypeScript ecosystem.

In the first stage, good candidates will be hired for small, freelance projects. We work in 30-hour sprints, which are paid at $150-200 USD per sprint. If everything goes fine, this could be a full time job.

## Position: Full Stack Engineer (TypeScript)

We're looking for developers with experience across the stack using TypeScript, including:
* Frontend frameworks (React, Vue, Angular, or similar)
* Backend with Node.js/TypeScript
* RESTful APIs and/or GraphQL
* Database integration (SQL or NoSQL)
* Modern development tooling (npm/yarn, build tools, testing frameworks)

## Application Process

In the application form, I request a link to a GitHub repo to see the results of the following technical challenge:

## General Requirements for the Challenge

1. Create an empty Github repo.
2. Do not push anything to the main branch.
3. Create a PR with all the code (do not merge it, keep it open for my review).
4. Using AI to accelerate coding is fine.
5. Record a code walkthrough and a demo of your application and paste the link to the video in the PR description. 5 min max.

## Challenge for Full Stack Engineers

#### Objective
Build a simple Order Management System with both frontend and backend components using TypeScript. The backend should handle CRUD operations and support pagination, while the frontend should allow users to interact with the order data seamlessly.

#### Requirements

###### Backend (Node.js + TypeScript)
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

4. **Tech Stack**
   - Node.js with TypeScript
   - Express.js, Fastify, or similar framework
   - Any database (PostgreSQL, MongoDB, or in-memory for simplicity)
   - Proper TypeScript types/interfaces for all models and API contracts

###### Frontend (TypeScript)
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

6. **Tech Stack**
   - React, Vue, Angular, or similar TypeScript framework
   - Type-safe API client (axios with types, fetch with types, or similar)
   - Proper TypeScript types/interfaces for all components and data

###### Bonus Points
- **Backend**: Add filtering by `status` for `GET /orders`.
- **Frontend**: Add a filter option to view orders by `status`.
- **Testing**: Include basic unit tests for both frontend components and backend endpoints (Jest, Vitest, or similar).
- **Documentation**: Add a comprehensive README with setup instructions for both frontend and backend.
- **Type Safety**: Shared types between frontend and backend (monorepo setup or published types package).
- **Code Quality**: ESLint/Prettier configuration, proper error handling.
- **Docker**: Docker setup for easy local development.

## How to Apply

When the code is ready, apply [here](https://docs.google.com/forms/d/e/1FAIpQLSdmPAcFIoH1ap6YhJmR4KCvP0s1h9fUfFMITcevS09wioRlCg/viewform?usp=header)


