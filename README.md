# 🍽️ Canteen Demand Predictor

**A Web-Based Canteen Management, Sales Analytics, Demand Visualization & Food Waste Reduction System**

Canteen Demand Predictor is a web-based application designed to help college canteens manage menu items, record sales orders, visualize demand patterns, analyze performance, and identify opportunities to reduce food waste.

The application provides an interactive dashboard with sales metrics, menu management, order tracking, statistical visualizations, demand estimates, and preparation recommendations through a simple and responsive user interface.

> **Project Type:** Data Analytics & Visualization Web Application  
> **Domain:** Canteen Management, Data Analytics & Food Waste Reduction  
> **Primary Use Case:** College Canteen Operations

---

## ✨ Key Features

### 1. 📊 Dashboard Overview
- Displays total revenue and units sold.
- Shows average daily demand per menu item.
- Identifies items with potentially low demand.
- Visualizes sales trends using a line chart.
- Displays category-wise demand using a doughnut chart.
- Highlights the top five items based on demand.
- Shows alerts for menu items that may require preparation adjustments.

### 2. 🍛 Menu Item Management
Implements CRUD (Create, Read, Update, Delete) operations for managing canteen menu items.

- Add new food and beverage items.
- View the menu in a tabular format.
- Edit existing menu item details.
- Delete menu items.
- Search items by name or category.
- Manage category, price, average daily demand, preparation time, and availability.

**Supported categories:**
- Veg
- Non-Veg
- Beverage
- Snack

**Availability options:** All Day, Morning, Afternoon, and Evening.

### 3. 🧾 Order Management
- Add sales order records.
- Select items from the available menu.
- Automatically populate item prices.
- Enter quantity, weekday, and time slot.
- Calculate revenue automatically using quantity × price.
- Filter order records by weekday.
- Delete order records.
- Display order counts and revenue totals for filtered records.

### 4. 📈 Demand Visualization
Provides multiple chart types for exploring menu demand and sales data.

| Visualization | Purpose |
|---|---|
| Line Chart | Compare demand patterns across weekdays |
| Bar Chart | Compare average demand across menu items |
| Scatter Plot | Explore the relationship between price and demand |
| Histogram | Group menu items into demand ranges |
| Horizontal Bar Chart | Rank menu items by demand |
| Radar Chart | Compare average demand across categories |

Additional visualizations include:
- Peak-hour sales analysis
- Day-wise sales comparison
- Revenue distribution by category

### 5. 🔍 Data Analysis
- Calculates total recorded revenue.
- Displays the number of active menu items.
- Calculates average demand per menu item.
- Identifies the highest-demand menu item.
- Displays a seven-day demand estimate chart.
- Compares menu item prices and demand.
- Generates an item-wise analysis table.
- Estimates weekly revenue using average demand and price.
- Displays demand efficiency percentages using progress bars.

### 6. ♻️ Waste Reduction Suggestions
Provides rule-based recommendations intended to help canteen operators improve food preparation planning.

- Identifies items with relatively low demand.
- Estimates potential waste exposure using predefined assumptions.
- Compares demand with estimated preparation quantities.
- Highlights high-demand products that may require increased preparation.
- Provides suggestions for adjusting preparation quantities.
- Displays demand-versus-preparation charts.
- Highlights potentially busy time slots and weekdays.

**Goal:** Reduce unnecessary food preparation, improve availability, and support more efficient canteen operations.

---

## 🛠️ Technologies Used

### Frontend Technologies

| Technology | Purpose |
|---|---|
| HTML5 | Defines the application structure and content |
| CSS3 | Provides styling, layouts, colors, tables, cards, and responsive design rules |
| JavaScript (Vanilla JS) | Implements application logic, event handling, calculations, CRUD operations, and rendering |
| Chart.js 4.4.1 | Creates interactive charts and data visualizations |

### External Library

**Chart.js**

The application loads Chart.js through a CDN:

`https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.js`

It is used for line, bar, doughnut, pie, scatter, radar, and other chart visualizations.

### Development Tools

The following tools can be used to develop and manage this project:

- Visual Studio Code — code editing
- Web browser — application execution and testing
- Git — version control
- GitHub — source code hosting
- GitHub Pages or Vercel — optional static website deployment

These are suggested development and deployment tools, not additional services implemented by the application itself.

---

## 🧠 Programming Concepts Used

### 1. HTML Concepts
- Semantic document structure
- Elements and attributes
- Forms and input fields
- Tables and data presentation
- Dropdown selections
- Buttons and click handlers
- Canvas elements for charts
- External JavaScript library integration

### 2. CSS Concepts
- CSS selectors and properties
- Flexbox layouts
- CSS Grid layouts
- Positioning and sticky side navigation
- Spacing and box model
- Hover and focus effects
- Transitions
- Reusable CSS classes
- Status badges and progress bars
- Color-coded alerts
- Responsive chart containers
- Basic horizontal overflow handling

### 3. JavaScript Concepts
- Variables using `let` and `const`
- Arrays and objects
- Functions and parameters
- Arrow functions
- Template literals
- DOM manipulation
- Event handling using `onclick`, `onchange`, and `oninput`
- Array methods such as `map()`, `filter()`, `reduce()`, `find()`, and `sort()`
- Spread syntax
- Conditional statements
- Loops and iteration
- String manipulation
- Number conversion and calculations
- Dynamic HTML generation
- Object property access
- Chart instance management
- Data aggregation and filtering

### 4. CRUD Operations

The menu management module demonstrates all four CRUD operations:

- **Create:** Add a new menu item.
- **Read:** Display and search existing menu items.
- **Update:** Edit menu item details.
- **Delete:** Remove menu items.

The order management module supports creating, displaying, filtering, and deleting order records.

### 5. Data Analytics Concepts
- Sales aggregation
- Revenue calculation
- Category-wise demand aggregation
- Day-wise sales analysis
- Peak-hour comparison
- Demand ranking
- Price-versus-demand analysis
- Histogram-based distribution analysis
- Estimated preparation surplus
- Threshold-based risk identification
- Basic trend visualization

---

## 📐 How the Application Works

1. **Initialize data:** JavaScript loads predefined menu items and sample order records.
2. **Render the dashboard:** Summary metrics, sales charts, top items, and alerts are generated.
3. **Manage the menu:** Users add, edit, search, and delete menu items.
4. **Record orders:** Users select menu items, enter quantities, and calculate order revenue.
5. **Analyze demand:** The application aggregates the available data and displays it through charts and tables.
6. **Generate suggestions:** Predefined rules identify low-demand and high-demand items and display preparation recommendations.
7. **Update the interface:** DOM manipulation and Chart.js refresh the relevant visualizations when the corresponding pages are opened.

---

## 🗂️ Project Structure

The current project can be maintained as a single HTML file:

```text
canteen-demand-predictor/
│
├── index.html
└── README.md
```

`index.html` contains the HTML markup, CSS styles, JavaScript logic, sample data, and Chart.js integration.

For a larger version, the application could be organized as:

```text
canteen-demand-predictor/
│
├── index.html
├── css/
│   └── style.css
├── js/
│   ├── app.js
│   ├── menu.js
│   ├── orders.js
│   ├── analytics.js
│   └── charts.js
├── assets/
└── README.md
```

The second structure is a suggested future refactoring, not the current file structure.

---

## 📊 Sample Data and Calculations

The current implementation contains:
- 10 predefined menu items.
- 13 predefined order records.
- Five weekdays: Monday to Friday.
- Five time slots.
- Four menu categories.

### Important calculations

**Order revenue**

`Revenue = Quantity × Item Price`

**Average menu demand**

`Average Demand = Sum of Item Demands ÷ Number of Menu Items`

**Estimated weekly revenue**

`Estimated Weekly Revenue = Average Daily Demand × Item Price × 5`

**Demand efficiency**

`Demand Efficiency (%) = Item Demand ÷ 150 × 100`

The demand efficiency metric uses 150 as a fixed reference value. It is not a measured operational efficiency score.

---

## ⚙️ Installation and Execution

### Run locally

1. Download or clone the repository.
2. Open the project folder in Visual Studio Code.
3. Open `index.html` in a modern web browser.
4. Navigate through the dashboard, menu, orders, demand charts, analysis, and waste reduction pages.

An extension such as Live Server can also be used to run the project through a local development server.

**Requirements:**
- A modern web browser.
- Internet connectivity to load Chart.js from its CDN.
- No backend server or database is required for the current demonstration.

---

## ⚠️ Current Limitations

The application is a frontend prototype that uses in-memory JavaScript data.

- Menu items and orders are predefined sample records.
- Changes are not persisted to a database.
- Refreshing the browser resets the application to its initial data.
- No user authentication or role-based access control is implemented.
- No backend API is connected.
- Demand estimates use simplified calculations rather than a trained machine learning model.
- Some charts use randomly generated values, so repeated renders may produce different results.
- Some waste and preparation figures are illustrative estimates, not verified measurements of actual food waste.
- The dashboard includes fixed labels and sample sales figures that are not all calculated from order records.
- The current CSS does not include comprehensive mobile breakpoints.

**Important:** Although the application uses demand-prediction and AI-driven terminology in its interface, the current implementation does not contain an AI model, machine learning pipeline, or real-time prediction service. Its recommendations are generated by predefined rules and simple arithmetic.

---

## 🚀 Future Enhancements

Possible improvements include:

- Integrate a backend using Python Flask, FastAPI, Node.js, or Spring Boot.
- Add MySQL, PostgreSQL, or MongoDB for persistent storage.
- Implement authentication and role-based access.
- Import historical order data from CSV or Excel files.
- Develop a trained demand forecasting model using historical sales data.
- Consider weekday, time slot, holidays, weather, and special events in demand forecasts.
- Calculate waste using actual prepared, sold, and discarded quantities.
- Add date-range filters and exportable analytics reports.
- Implement automated low-stock and overproduction alerts.
- Improve accessibility and mobile responsiveness.
- Add automated testing and production deployment.

These enhancements would help evolve the prototype into a more complete canteen analytics platform.

---

## 🎯 Learning Outcomes

This project demonstrates practical application of:

- Frontend web development
- Interactive dashboard design
- JavaScript-based CRUD operations
- Data structures and array processing
- Data visualization using Chart.js
- Basic descriptive analytics
- Revenue and demand calculations
- Rule-based recommendation logic
- UI event handling and dynamic rendering
- Data-driven decision support

---

## 📌 Project Summary

**Canteen Demand Predictor** is a frontend-based canteen analytics and management prototype that combines menu administration, order recording, sales visualization, demand analysis, and food waste reduction recommendations in one interface.

It provides a foundation for exploring how web technologies and data analytics can support more informed food preparation and canteen management decisions.

**Technologies:** HTML5 · CSS3 · JavaScript · Chart.js

**Status:** Frontend prototype with sample data

---

*Note: All sample records, demand figures, revenue estimates, and recommendations should be treated as demonstration data unless replaced with verified operational data.*
