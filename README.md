# Gett - Insights from Failed Orders

![image](https://github.com/user-attachments/assets/f6cc8b00-c41c-4e77-b98e-95b65ee807ee)

This project focuses on analyzing failed taxi orders from the Gett application. The goal is to understand the reasons behind order failures and identify patterns that could help improve the matching system. The analysis involves exploring various metrics such as reasons for failure, time to cancellation, and distribution of failed orders by hour.

<br>

Give this repository a ⭐ if you liked it, since it took me time to analyze and implement this. <br>
Made with ❤️ by <b>Om Rajesh Chitmalwar<b>

<br>

### 🗓️ Project Duration
March 2024 - March 2024

<br>

### 🔍 Key Features
#### 📂 Data Columns
1. data_orders
   - `order_datetime`: Time of the order
   - `origin_longitude`: Longitude of the order
   - `origin_latitude`: Latitude of the order
   - `m_order_eta`: Time before order arrival
   - `order_gk`: Order number
   - `order_status_key`: Status, an enumeration consisting of:
     - `4`: Cancelled by client
     - `9`: Cancelled by system, i.e., a reject
   - `is_driver_assigned_key`: Whether a driver has been assigned
   - `cancellation_time_in_seconds`: How many seconds passed before cancellation

<br>

2. data_offers
   - `order_gk`: Order number, associated with the same column from the orders data set
   - `offer_id`: ID of an offer
  
<br> 

### 🛠️ Data Analysis Steps
#### 1. Distribution of Orders by Reasons for Failure
   - Build the distribution of orders according to reasons for failure: cancellations before and after driver assignment, and reasons for order rejection.
   - Analyze the resulting plot to determine which category has the highest number of orders.

#### 2. Distribution of Failed Orders by Hours
   - Plot the distribution of failed orders by hours.
   - Identify if there is a trend that certain hours have an abnormally high proportion of one category or another.
   - Determine the hours with the highest number of fails and provide possible explanations.

#### 3. Average Time to Cancellation Analysis
   - Plot the average time to cancellation with and without driver, by the hour.
   - Remove any outliers from the data for better insights.
   - Draw conclusions from the plot.

#### 4. Distribution of Average ETA by Hours
   - Plot the distribution of average ETA by hours.
   - Provide an explanation for the resulting plot.

#### 5. BONUS: Hexagon Visualization
   - Using the h3 and folium packages, calculate how many size 8 hexes contain 80% of all orders from the original data sets.
   - Visualize the hexes on a map, coloring them by the number of fails.

<br>

### 💼 Skills Utilized
- Data Cleaning and Manipulation 🧹
- Data Analysis 📊
- Data Visualization 🎨
- Python Programming 🐍
- Statistical Analysis 📊

<br>

### 📥 Getting Started
1. Clone the repository: <pre> git clone https://github.com/omrajeshchitmalwar/Gett-Insights-From-Failed-Orders.git
2. Navigate to the project directory: <pre> cd Gett-Insights-From-Failed-Orders

<br>

### 🌟 Acknowledgements
Special thanks to the data providers and the Python community for their support and documentation.

<br>

### 📬 Contact
For any questions or feedback, please reach out to omrajeshchitmalwar@gmail.com.

