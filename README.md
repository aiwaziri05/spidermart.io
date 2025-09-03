# SpiderMart – Multi-Vendor SaaS E-commerce Platform (Frontend MVP)

![React](https://img.shields.io/badge/react-18-blue)
![Vite](https://img.shields.io/badge/vite-v5.4-green)
![TailwindCSS](https://img.shields.io/badge/tailwind-v4-teal)
![License](https://img.shields.io/badge/license-MIT-yellow)

---

## Table of Contents
- [Project Overview](#project-overview)
- [Goals & Objectives](#goals--objectives)
- [Target Users](#target-users)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation & Setup](#installation--setup)
- [Project Structure](#project-structure)
- [Homepage & Hero Section](#homepage--hero-section)
- [Design Guidelines](#design-guidelines)
- [Performance & UI Enhancements](#performance--ui-enhancements)
- [Non-Functional Requirements](#non-functional-requirements)
- [License](#license)

---

## Project Overview
SpiderMart is a **scalable SaaS multi-vendor e-commerce platform** focused on promoting Nigerian culturally unique products (leather, textiles, shoes, clothes, and bags) to both local and global markets.  

This frontend MVP is built with **React + Vite + Tailwind CSS**, structured for future **Next.js migration**. Backend features (authentication, payments, orders, vendor management) are mocked for now.

---

## Goals & Objectives
- Provide vendors with tools to **register and showcase** their cultural products.  
- Offer customers a **modern, intuitive shopping experience**.  
- Ensure the frontend is **modular, scalable, and SaaS-ready**.  
- Implement a **bento grid hero section** and modern navigation for an engaging homepage.  
- Prepare for seamless **Next.js migration** (SSR, SEO, multi-tenant SaaS architecture).  

---

## Target Users
| User Role    | Description                                                                   |
| ------------ | ----------------------------------------------------------------------------- |
| **Customer** | End users who browse, search, and purchase Nigerian cultural products.        |
| **Vendor**   | Artisans and suppliers who register, list, and manage products/stores.        |
| **Admin**    | Platform operators (future scope) who manage vendors, products, and policies. |

---

## Features

### Customer Features
- Browse products by category with images, names, and prices (mock/demo data)  
- Search & filter products dynamically  
- Wishlist functionality stored locally (Redux/Zustand)  
- Add to cart & checkout UI ready for backend integration  
- Order history page with demo data  
- Google Sign-In (OAuth2) UI implemented; backend exchange mocked

### Vendor Features
- Vendor registration & onboarding via **“Sell on SpiderMart”** CTA  
- Manage products: add, edit, remove (local state + mock API)  
- View incoming orders (dashboard with demo data)  
- Sales dashboard with charts/graphs (mock data)

> ⚠️ Admin panel is out of scope for this frontend MVP

---

## Tech Stack
- **Frontend:** React 18 + Vite  
- **Styling:** Tailwind CSS v4  
- **State Management:** Redux Toolkit or Zustand  
- **API Layer:** Axios stubs (mock/demo endpoints)  
- **Auth:** Google OAuth2 UI  
- **Charts/Graphs:** Recharts (for dashboards)  

---

## Installation & Setup
1. Clone the repo:
```bash
git clone https://github.com/username/spidermart.git

cd spidermart
npm install
npm run dev


```
## Project Structure

```text
📁 /src
│
├─ 📁 components   # Reusable UI components (cards, forms, modals, nav, hero grid)
├─ 📁 features     # Feature modules (cart, wishlist, checkout, vendor-dashboard)
├─ 📁 pages        # Page-level components (Next.js compatible)
├─ 📁 services     # Axios clients and API stubs
├─ 📁 stores       # Redux slices / Zustand stores
├─ 📁 styles       # Tailwind CSS config & global styles
└─ 📁 utils        # Helper functions (formatting, validation)
```

## Homepage & Hero Section

- **Hero Slider (2/3 width, top-left):** rotating banners with CTAs  
- **Tall Right Column (1/3 width, spanning two rows):** top & bottom category highlights  
- **Bottom Row:** Leather Goods block + Cultural Discovery block  

**Responsive Layout:**  
- Mobile-first design: slider full-width, stacked columns, 2-column grid for bottom blocks

## Non-Functional Requirements

- **Performance:** Load under 2s on 3G, Lighthouse score > 90  
- **Responsiveness:** Mobile-first, works on all screen sizes  
- **Accessibility:** WCAG-compliant, keyboard-friendly, proper alt text  
- **Security:** HTTPS, SSL, safe token handling  
- **Scalability:** Modular, SaaS-ready, prepared for Next.js migration  
- **Code Standards:** Use plain JSX (no TypeScript required)

## License

This project is licensed under the **MIT License**.  
© 2025 Abdullahi Idi Waziri

