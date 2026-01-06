# Meridian Retail Platform

An intelligent full-stack Next.js application for Meridian Retail Group, providing role-based dashboards for different profile levels within the company.

## Features

### Profile-Based Dashboards

1. **C-Level Executive Dashboard**
   - Overall conversion trends (online + store)
   - Customer loyalty & repeat purchase trends
   - Inventory health monitoring
   - Employee turnover & engagement trends
   - Revenue at risk analysis
   - Strategic alerts and reports

2. **Marketing Manager Dashboard**
   - Browsing vs buying gap analysis
   - Cart abandonment patterns
   - Discount sensitivity by segment
   - Category-level return reasons
   - Campaign performance tracking
   - Action items for social media and promotions

3. **Operations Manager Dashboard**
   - Real-time inventory by SKU
   - Sales velocity tracking
   - Lead times and supplier reliability
   - Stockout and overstock risk alerts
   - Inventory vs demand mismatch analysis

4. **Sales Associate Dashboard**
   - Customer lookup by email or phone
   - Customer profile and purchase history
   - Recent browsing and purchase intent
   - Special discount offers for new online customers
   - Cart and return information

5. **HR Manager Dashboard**
   - Turnover by role/store/region
   - Training completion status
   - Schedule predictability metrics
   - Employee stress vs customer experience correlation
   - Training gap analysis

## Tech Stack

- **Next.js 14** - React framework with App Router
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first CSS framework
- **Recharts** - Charting library for data visualization
- **Lucide React** - Icon library

## Getting Started

### Prerequisites

- Node.js 18+ installed
- npm or yarn package manager

### Installation

1. Install dependencies:
```bash
npm install
```

2. Run the development server:
```bash
npm run dev
```

3. Open [http://localhost:3000](http://localhost:3000) in your browser

### Build for Production

```bash
npm run build
npm start
```

## Project Structure

```
├── app/
│   ├── dashboard/
│   │   └── [profile]/     # Dynamic route for profile dashboards
│   ├── globals.css        # Global styles
│   ├── layout.tsx         # Root layout
│   └── page.tsx           # Profile selection page
├── components/
│   ├── dashboards/        # Profile-specific dashboard components
│   └── shared/            # Reusable UI components
├── data/                  # JSON data files
│   ├── customer-data.json
│   ├── inventory-data.json
│   └── employee-data.json
└── lib/
    └── data.ts            # Data access utilities
```

## Data Files

The application uses three JSON data files:

1. **customer-data.json** - Customer information, purchase history, browsing behavior
2. **inventory-data.json** - Product inventory, stock levels, sales velocity
3. **employee-data.json** - Employee information, training status, turnover data

## Usage

1. **Select Profile**: On the home page, select your role/profile
2. **View Dashboard**: Each profile shows relevant KPIs, alerts, and reports
3. **Sales Associate**: Use the customer lookup to search by email or phone
4. **Monitor Alerts**: Critical alerts are highlighted for immediate attention
5. **Review Reports**: Access detailed reports for strategic decision-making

## Future Enhancements

- Integration with Amazon Bedrock AI for intelligent insights
- Real-time data updates via API
- User authentication and authorization
- Advanced filtering and search capabilities
- Export functionality for reports

## License

This project is proprietary software for Meridian Retail Group.

