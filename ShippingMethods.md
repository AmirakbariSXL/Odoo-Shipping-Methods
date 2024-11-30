# Odoo-Shipping-Methods



# 5 Shipping Methods in Odoo Without Coding

This document provides a comprehensive guide to 5 different shipping methods in Odoo that can be implemented without any need for custom module development or coding. Each method is built-in and leverages Odoo's existing features to streamline the shipping process in your business.

## 1. **Use Odoo's Built-in Shipping Methods**

Odoo offers a default set of shipping methods that can be configured to match your business's needs. These methods allow you to assign shipping charges, delivery times, and conditions to your orders without needing to write custom code.

### Steps to Configure Built-in Shipping Methods:
1. **Go to the Inventory App**:
   - Navigate to the **Inventory** app from the Odoo dashboard.
   
2. **Access Shipping Method Configuration**:
   - Click on the **Configuration** menu on the top bar and then select **Shipping Methods**.
   - Here, you can see a list of existing shipping methods.

3. **Create or Edit a Shipping Method**:
   - Click the **Create** button to add a new shipping method or choose an existing one to modify.
   - A form will open where you can configure the shipping method.

4. **Configure the Shipping Method**:
   - **Name**: Give the shipping method a descriptive name (e.g., "Standard Shipping", "Express Shipping").
   - **Carrier**: Choose the carrier if you’re linking to an external service, or select the custom carrier option for an internal shipping method.
   - **Price Calculation**: You can define how shipping costs are calculated (flat rate, weight-based, etc.).
   - **Delivery Time**: Set an expected delivery time for this shipping method.
   - **Applicable Sales Orders**: You can specify which types of orders (e.g., domestic or international) this shipping method applies to.

5. **Link to Products**:
   - Under **Sales**, link this shipping method to your products by selecting it in the shipping tab for each sales order or product.

6. **Save Your Configuration**:
   - Once you've completed the setup, save the shipping method and it will be available for use during order processing.

### Outcome:
This method allows you to offer different shipping options (e.g., standard, express) and apply them to customer orders. It is suitable for businesses that handle shipments using their own internal delivery services.

---

## 2. **Use Third-Party Shipping Integrations (External Carrier Integration)**

Odoo offers integrations with third-party shipping carriers like FedEx, UPS, DHL, and many more. These integrations allow you to automatically calculate shipping costs, print shipping labels, and track shipments directly from within Odoo, without any need for coding.

### Steps to Configure Third-Party Carrier Integrations:
1. **Go to the Inventory App**:
   - From the Odoo dashboard, open the **Inventory** app.

2. **Activate Shipping Providers**:
   - Navigate to **Configuration** > **Shipping Providers**. If you don’t see this option, ensure that the integration module for the shipping provider (e.g., FedEx, UPS) is installed.
   - Click on **Activate Carrier** to begin the integration process.

3. **Enter API Credentials**:
   - Once the provider is activated, you’ll need to enter API credentials for the carrier service.
   - These credentials are typically available in your carrier’s account portal (e.g., FedEx or UPS) and include the API key, username, and password.

4. **Configure Shipping Methods**:
   - After integrating the carrier, go to **Inventory** > **Shipping Methods**.
   - You’ll see a new shipping method option tied to the third-party provider you configured (e.g., “FedEx Ground” or “UPS Standard”).
   - Configure the shipping method based on your requirements (delivery time, pricing rules, etc.).

5. **Use the Shipping Method**:
   - When processing sales orders, Odoo will now allow you to automatically select the third-party carrier and calculate real-time shipping rates for each order.

6. **Track Shipments**:
   - Once the order is shipped, you can track the shipment directly from within Odoo by using the tracking number provided by the carrier.

### Outcome:
This method is ideal for businesses that rely on external logistics companies for delivery and need seamless integration between Odoo and third-party shipping providers for automatic cost calculation, label printing, and shipment tracking.

---

## 3. **Use Weight-Based Shipping**

Weight-based shipping allows businesses to calculate shipping costs dynamically based on the total weight of the products in an order. This method is particularly useful for businesses that sell physical products with varying weights.

### Steps to Set Up Weight-Based Shipping:
1. **Go to the Inventory App**:
   - Open the **Inventory** app from the Odoo dashboard.

2. **Create a Shipping Method**:
   - Navigate to **Configuration** > **Shipping Methods** and click **Create**.

3. **Set the Shipping Calculation Method**:
   - In the **Shipping Method** form, choose **Weight-Based** as the calculation method.
   - Define the **shipping price based on weight ranges** (e.g., products weighing 0–5 kg will cost $5 to ship, while products weighing 5–10 kg will cost $10).

4. **Define Weight Ranges**:
   - Under the **Price Computation** tab, set different pricing rules for each weight range.
   - Example: 
     - Weight range 0–5 kg: $5 shipping cost.
     - Weight range 5–10 kg: $10 shipping cost.

5. **Assign the Shipping Method**:
   - Assign this shipping method to your sales orders so that when products are sold, the shipping cost is calculated based on the total weight of the items in the order.

### Outcome:
This approach is ideal for businesses that ship physical products and want a straightforward, weight-based pricing model for shipping. The system will automatically calculate the shipping cost based on the total weight of each order.

---

## 4. **Use Free Shipping**

Offering free shipping can be an effective sales tactic for increasing order volume. Odoo allows you to set up free shipping based on certain conditions, such as a minimum order amount or specific regions.

### Steps to Set Up Free Shipping:
1. **Go to the Sales App**:
   - From the Odoo dashboard, open the **Sales** app.

2. **Create a Free Shipping Method**:
   - Navigate to **Configuration** > **Shipping Methods** and click on **Create**.
   - Name the shipping method “Free Shipping”.

3. **Set Conditions for Free Shipping**:
   - In the shipping method form, configure the condition for offering free shipping. Common conditions include:
     - **Minimum order value**: Free shipping can be applied if the total order value exceeds a specific amount (e.g., $100).
     - **Sales team**: You can limit free shipping to orders processed by a specific sales team.
     - **Customer group**: Offer free shipping to specific customer groups (e.g., VIP customers).

4. **Activate and Assign the Method**:
   - Save the shipping method and assign it to your sales process.
   - Now, when customers meet the conditions, free shipping will automatically be applied to their orders.

### Outcome:
This shipping method is great for businesses that want to offer an incentive like free shipping for orders above a certain value, or for specific customer types. Odoo automates this process based on the rules you set.

---

## 5. **Use Local Delivery or Pick-up Option**

If your business has a physical store or local delivery system, you can configure a local delivery or pick-up option for customers to either pick up their orders in-store or have them delivered within a specific local area.

### Steps to Set Up Local Delivery or Pick-up:
1. **Go to the Inventory App**:
   - From the Odoo dashboard, open the **Inventory** app.

2. **Create a Local Delivery/Pick-up Shipping Method**:
   - Navigate to **Configuration** > **Shipping Methods** and click on **Create**.
   - Name the shipping method “Local Delivery” or “In-Store Pick-Up”.

3. **Define Delivery Conditions**:
   - Specify whether this option is available for specific locations, customer types, or regions.
   - You can also set specific delivery fees or offer it for free depending on the condition.

4. **Assign to Sales Orders**:
   - When processing sales orders, select this option for local delivery or in-store pick-up, and the system will update the order accordingly.

### Outcome:
This option is ideal for businesses that have a physical presence and want to offer local customers the ability to pick up their orders in person or have them delivered locally.

