# 🍽️ MealBridge  

MealBridge is a purpose-built platform that connects **donors** with **NGOs** to reduce food waste and support communities in need.  
It streamlines the **end-to-end journey of surplus meal donations**—from posting and discovery to claiming, pickup, and completion—while ensuring clarity, accountability, and ease of use for all stakeholders.  

---

## 🚀 Features  

### 👤 Donor  
- Create and manage food donations with details (name, category, quantity, expiry date, pickup address, etc.).  
- Track donation statuses in a personalized dashboard (**Available, Expired, Completed**).  
- Get notifications when NGOs claim donations.  
- Monitor interest with “Claimed by X” indicators.  
- Edit donation details anytime.  

### 🏢 NGO  
- Browse and search available donations using filters (category, name, date).  
- Place claims with required quantities and notes.  
- Track claims with statuses (Pending, Approved, Completed).  
- View donor details (name, contact, pickup address).  

### 🛡️ Admin (optional)  
- Monitor donations, claims, users, and categories.  
- Manage flagged cases (expired donations, excessive claims).  
- Seed and maintain categories for better discoverability.  

---

## 🔄 Core Workflow  

1. **Donation Creation**  
   - Donors submit new donations with category, quantity, expiry, and pickup location.  
   - The system tracks **Total Quantity** and **Available Quantity**.  

2. **Discovery & Claiming**  
   - NGOs browse/search available donations.  
   - Multiple NGOs can claim a single donation until availability is exhausted.  

3. **Notifications & Coordination**  
   - Donors receive claim notifications with NGO details.  
   - Donors mark claims as **Completed** after handover.  

4. **Completion & Status Logic**  
   - **Available** → Expiry date valid & quantity > 0.  
   - **Completed** → Available quantity = 0.  
   - **Expired** → Expiry date passed.  

---

## 📊 Data Model  

- **Users**: Donor / NGO / Admin with name, email, contact, address.  
- **FoodDonation**: Name, Category, Quantity, Available Quantity, Expiry Date, Pickup Location, Status.  
- **FoodClaim**: Claim Quantity, Status, Notes, Claim Date, Pickup Date.  

**Relationships**  
- One Donor → Many Donations.  
- One Donation → Many Claims.  
- One NGO → Many Claims.  

---

## 🛠️ Tech Stack  

- **Backend**: .NET Core   
- **Frontend**: Razor Views 
- **Database**: SQL Server 
- **Auth**: Session-based authentication with role-based access  

---

## 📣 Impact  

- Reduce food waste.  
- Empower NGOs to serve communities better.  
- Build transparency and trust in food redistribution.  
---

## 🤝 Contributing  

Contributions are welcome!  
- Fork the repo  
- Create a feature branch  
- Submit a pull request 🚀  

---

## 📜 License  

This project is licensed under the **MIT License**.  

---

### 🌟 Summary  

MealBridge brings **donors, NGOs, and communities together** through a streamlined, transparent, and user-friendly platform.  
It ensures accurate donations, efficient NGO discovery, smooth claims & handovers, and meaningful social impact—while being scalable and extensible for the future.  

---

