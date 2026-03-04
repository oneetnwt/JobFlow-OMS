# JPCH Multi-Tenant Job Order & Inventory Monitoring System

> **Note:** This is a school project submitted for the **Web Systems and Technologies** course.

## Short Description

JPCH is a cloud-based, multi-tenant Job Order and Inventory Management System developed using the Laravel Framework. It centralizes job order tracking, material allocation, and status monitoring to eliminate data silos in construction companies, maintenance departments, and facilities management teams.

## Features

- **Multi-Tenant Architecture** – Each organization operates in an isolated environment with its own data and configuration.
- **Job Order Management** – Create, assign, approve, and track job orders across departments.
- **Inventory Monitoring** – Manage stock levels, approve material withdrawals, and track material movement.
- **Role-Based Access Control** – Distinct roles including Tenant Admin, Staff/Technician, Inventory Officer, Viewer/Manager, and Super Admin.
- **Dashboards & Reports** – Real-time visibility into project progress, inventory status, and job order history.
- **Payroll & Time Logging** – Staff can log time spent on tasks for payroll and productivity tracking.
- **Subscription Management** – Super Admin can manage tenants, approve subscriptions, and enable or disable accounts.

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | PHP 8.x, Laravel 11 |
| Frontend | Blade Templates, Vite, Tailwind CSS |
| Database | MySQL |
| Authentication | Laravel Breeze / Sanctum |
| Testing | Pest PHP |
| Package Manager | Composer, npm |

## Installation / Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/jpch-oms.git
   cd jpch-oms
   ```

2. **Install dependencies**
   ```bash
   composer install
   npm install
   ```

3. **Configure environment**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. **Set up your database** in `.env`, then run migrations and seeders:
   ```bash
   php artisan migrate --seed
   ```

5. **Build frontend assets**
   ```bash
   npm run dev
   ```

6. **Start the local server**
   ```bash
   php artisan serve
   ```

   The application will be available at `http://localhost:8000`.

## Usage

1. **Super Admin** logs in to create and manage tenant accounts.
2. **Tenant Admin** sets up the company profile, configures settings, and invites users.
3. **Staff / Technicians** submit job orders and update task progress.
4. **Inventory Officers** handle material requests, stock updates, and withdrawal approvals.
5. **Viewers / Managers** monitor dashboards and generate reports without editing data.

## Project Status

> **Under Development** – Core modules for job order management and multi-tenancy are actively being built. Features and database structure are subject to change.

## License

This project is proprietary software. Unauthorized copying, distribution, or modification is not permitted without explicit written consent from the project owner.
