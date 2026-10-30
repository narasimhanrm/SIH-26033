# Smart India Hackathon Workshop
# Date: 30-10-2026
## Reference Number: 26019371
## Name: NARASIMHAN RM

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.


## Proposed Solution

### FarmLink Direct — A Demand-First Agricultural Supply Network

FarmLink Direct is a digital agricultural marketplace designed to reduce unnecessary intermediaries by changing the traditional supply-chain model from **"farmer produces → intermediary searches for buyer"** to **"buyer creates demand → platform aggregates suitable farmers → optimized delivery."**

Instead of requiring individual farmers to find buyers, consumers, retailers, restaurants, institutions and bulk purchasers can post their requirements on the platform, including crop, quantity, quality, location and required delivery date.

The platform then identifies suitable farmers and Farmer Producer Organizations (FPOs) in nearby regions and combines compatible orders from multiple farmers when necessary. This creates a digital aggregation layer without requiring several physical intermediaries.

The system provides:

- Direct farmer-to-buyer discovery.
- Buyer demand posting and advance order matching.
- Aggregation of produce from multiple nearby farmers.
- Transparent farm-gate price and buyer price information.
- Shared transportation for compatible orders.
- AI-based demand forecasting.
- AI-assisted buyer-farmer matching.
- Route optimization for collection and delivery.
- Digital order tracking and payment records.
- Quality and quantity verification at collection points.
- Digital transaction history for farmers and buyers.

### How It Addresses the Problem

The major issue is not simply that intermediaries exist, but that multiple layers can appear between production and final consumption without adding proportional value.

FarmLink Direct attempts to reduce these unnecessary layers by creating a transparent digital coordination layer between producers and buyers.

For example, instead of:

**Farmer → Local Trader → Wholesaler → Distributor → Retailer → Consumer**

the platform aims to enable:

**Farmer/FPO → FarmLink Network → Buyer/Consumer**

For larger orders, several nearby farmers can be grouped together:

**Multiple Farmers → Digital Aggregation → Shared Logistics → Bulk Buyer**

The platform does not attempt to completely eliminate every intermediary. Transporters, collection centers, quality inspectors and other service providers can still participate when they provide genuine value. The objective is to make every participating service visible, measurable and economically transparent.

### Innovation and Uniqueness

The core innovation is the **Demand-First Agricultural Network**.

Most digital agricultural marketplaces primarily depend on farmers listing their available produce. FarmLink Direct reverses this process.

A buyer first creates a demand request. The platform then determines:

1. Which farmers can satisfy the requirement.
2. Whether multiple farmers should be aggregated.
3. Whether the requested quantity is available locally.
4. The estimated farm-gate and final delivery cost.
5. The most efficient collection and delivery route.
6. Whether the order should be fulfilled immediately or scheduled.

This creates a **"virtual procurement network"** that can coordinate small farms as if they were one larger supplier.

A transparent price breakdown also shows the approximate distribution of the transaction value:

**Buyer Payment = Farmer Value + Logistics Cost + Platform/Service Cost**

This allows farmers and buyers to understand where the money goes instead of relying on an opaque chain of negotiations.

---

# Technical Approach

## System Architecture

The proposed system consists of five major layers:

### 1. Farmer and Buyer Layer

Farmers/FPOs can:

- Register their farms or organizations.
- Add available crops.
- Specify quantity, expected harvest date and location.
- Update availability.
- Accept or reject matched orders.
- Track payments and deliveries.

Buyers can:

- Search available produce.
- Create demand requests.
- Specify quantity, quality, location and delivery date.
- Place orders.
- Track fulfillment and delivery.

### 2. Matching and Aggregation Engine

The platform maintains two major data streams:

**Supply Data**
- Crop type
- Quantity
- Farm location
- Harvest date
- Quality information
- Historical availability

**Demand Data**
- Crop required
- Quantity
- Quality
- Buyer location
- Required date
- Historical demand

A matching engine compares these datasets and identifies suitable farmer-buyer combinations.

When one farmer cannot satisfy an order, the system can combine compatible quantities from several nearby farmers.

### 3. AI Demand Forecasting

Historical transactions, seasonal patterns, crop availability, regional demand and market trends can be used to estimate future demand.

The forecasting module can generate predictions such as:

- Expected demand for a crop.
- Expected demand by region.
- Upcoming high-demand periods.
- Possible surplus or shortage conditions.

This information can help farmers and FPOs make better production and selling decisions.

### 4. Logistics Optimization

Once orders are confirmed, the logistics module groups compatible deliveries and calculates efficient collection and delivery routes.

The system considers:

- Farmer locations.
- Buyer locations.
- Quantity of produce.
- Vehicle capacity.
- Distance.
- Delivery deadlines.
- Multiple collection points.

The objective is to reduce unnecessary trips, transportation costs and empty vehicle movement.

### 5. Transparent Settlement Layer

Every completed transaction generates a digital record containing:

- Quantity supplied.
- Agreed farmer price.
- Logistics cost.
- Platform/service charges.
- Final buyer price.
- Payment status.

This creates a transparent transaction trail and allows farmers to understand their actual earnings.

## Suggested Technology Stack

### Frontend
- HTML
- CSS
- JavaScript
- React.js

### Backend
- Python
- FastAPI

### Database
- PostgreSQL

### AI/ML
- Python
- Scikit-learn
- Pandas
- NumPy

### Maps and Logistics
- OpenStreetMap
- Routing API
- Graph-based route optimization

### Authentication and Security
- JWT-based authentication
- Role-based access control
- HTTPS
- Secure password hashing

### Deployment
- Docker
- Cloud-based deployment

## System Flow

<img width="2430" height="1496" alt="farmlink_technical_architecture" src="https://github.com/user-attachments/assets/914991f0-07a6-4b48-a044-f9057a4212e4" />
<img width="2430" height="1326" alt="farmlink_ai_logistics_loop" src="https://github.com/user-attachments/assets/29604dd0-9e3f-4806-836a-3dad7e232523" />
<img width="2430" height="1326" alt="farmlink_demand_first_workflow" src="https://github.com/user-attachments/assets/656415a3-f582-4f12-b1c0-80d78304758a" />


## Implementation Methodology

### Phase 1 — Digital Marketplace

Develop farmer, FPO and buyer registration along with crop listing, demand creation and order management.

### Phase 2 — Matching Engine

Develop the farmer-buyer matching algorithm using crop, quantity, location, quality and delivery date.

### Phase 3 — Aggregation

Allow multiple nearby farmers to collectively fulfill a larger order.

### Phase 4 — Logistics Optimization

Integrate mapping and routing services to calculate efficient collection and delivery routes.

### Phase 5 — AI Forecasting

Train demand forecasting models using historical and seasonal data.

### Phase 6 — Prototype Testing

Test the system using simulated agricultural supply and demand data from multiple regions and compare:

- Farmer realization price.
- Buyer final price.
- Transportation distance.
- Number of intermediary stages.
- Order fulfillment time.
- Logistics cost.

---

# Feasibility and Viability

## Feasibility

The proposed system is technically feasible because its major components can be implemented using existing web, database, mapping and machine-learning technologies.

The initial prototype can operate with manually entered or publicly available agricultural datasets. GPS-based location information can be used to calculate distances between farms, collection points and buyers.

The AI components do not require highly complex models during the initial stage. Demand forecasting can begin with statistical and machine-learning approaches and become more sophisticated as transaction data increases.

The system can also be deployed incrementally instead of requiring nationwide implementation from the beginning.

## Potential Challenges and Risks

### 1. Farmer Digital Literacy

Some farmers may have limited experience with digital platforms.

**Solution:** Provide a simple regional-language interface and allow FPOs or assisted collection centers to enter information on behalf of farmers.

### 2. Inaccurate Supply Information

Farmers may not always know the exact quantity available.

**Solution:** Allow quantity updates and introduce collection-stage verification before final settlement.

### 3. Quality Variation

Produce from different farms may have different quality levels.

**Solution:** Introduce standardized quality categories and digital quality verification during collection.

### 4. Logistics Complexity

Collecting produce from multiple farms can increase operational complexity.

**Solution:** Use route optimization and vehicle-capacity constraints to determine whether aggregation is economically practical.

### 5. Demand Forecasting Errors

AI predictions cannot guarantee future demand.

**Solution:** Present forecasts as decision-support information rather than guaranteed predictions and continuously retrain models using new transaction data.

### 6. Trust and Adoption

Farmers and buyers may initially prefer existing trading relationships.

**Solution:** Provide transparent transaction records, competitive pricing information, digital receipts and reliable order tracking to build trust gradually.

## Viability Strategy

The system can initially be deployed as a pilot in one agricultural region with selected FPOs and institutional buyers.

After validating the model, additional crops, regions, logistics providers and buyers can be added.

The platform can generate revenue through a small transparent service fee for successful transactions or optional logistics and analytics services rather than relying on hidden margins.

---

# Impact and Benefits

## Benefits to Farmers

- Greater access to direct buyers.
- Reduced dependence on unnecessary intermediaries.
- Better visibility of available market demand.
- Potentially higher realization of the final selling price.
- Ability to combine produce with other farmers for bulk orders.
- Digital transaction history.
- Demand forecasts for future planning.

## Benefits to Consumers and Bulk Buyers

- Potentially lower procurement costs.
- Direct access to producers and FPOs.
- Transparent pricing.
- Ability to submit specific quantity and quality requirements.
- Better order tracking.
- More predictable procurement.

## Economic Impact

The platform can reduce inefficiencies caused by fragmented procurement and transportation.

By aggregating supply digitally, small farmers can participate in larger orders that would normally be difficult to fulfill individually.

The transparent price breakdown can also help identify where excessive costs are introduced in the supply chain.

## Social Impact

The platform can improve digital participation of rural communities and provide farmers with greater visibility into market demand.

FPOs can act as digital aggregation partners, allowing small farmers to participate without individually handling large institutional orders.

## Environmental Impact

Logistics optimization can reduce:

- Unnecessary transportation.
- Duplicate trips.
- Empty vehicle movement.
- Fuel consumption.

Better demand forecasting can also help reduce avoidable overproduction and wastage caused by demand-supply mismatches.

---

# Research and References

The proposed solution is informed by research and existing agricultural digital infrastructure, including:

1. **National Agriculture Market (e-NAM)** — Government of India  
   Digital agricultural market infrastructure and electronic trading concepts.

2. **Ministry of Agriculture & Farmers Welfare, Government of India**  
   Information related to agricultural markets, Farmer Producer Organizations and agricultural supply chains.

3. **Digital India Programme** — Government of India  
   Digital infrastructure and technology adoption in public services.

4. **Food and Agriculture Organization of the United Nations (FAO)**  
   Research on food supply chains, agricultural markets, food loss and rural development.

5. **NITI Aayog**  
   Research and policy material related to agriculture, supply chains, farmer income and agricultural technology.

6. **OpenStreetMap**  
   Open geographic data that can be used for location and routing-based applications.

7. **Scikit-learn Documentation**  
   Machine-learning methods suitable for developing the demand forecasting prototype.

8. **Research Area: Agricultural Supply Chain Optimization**  
   Existing academic research on demand forecasting, vehicle routing, supply aggregation and agricultural logistics was considered while designing the proposed architecture.

The proposed system combines these concepts into a demand-first agricultural procurement network focused specifically on reducing unnecessary intermediary layers while preserving logistics, quality verification and other services that provide genuine value.
