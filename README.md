# visualizer



# 📊 Data Analysis & Visualization Project

print("📁 Dataset: Sales_data.csv")
print("😊 Ready to analyze your data!")
print("📈 You can explore, clean, analyze and visualize the dataset.")
print("🚀 Project started successfully!")

# ▶️ Run the main program
main()

📁 Dataset: Sales_data.csv
😊 Ready to analyze your data!
📈 You can explore, clean, analyze and visualize the dataset.
🚀 Project started successfully!

============================================================
========== Data Analysis & Visualization Project ==========
Please select an option:
1. Load Dataset
2. Explore Data
3. Perform DataFrame Operations
4. Handle Missing Data
5. Generate Descriptive Statistics
6. Data Visualization
7. Save Visualization
8. Exit
============================================================

# 📊 Step 6: Data Visualization

print("\n📈 == Data Visualization ==")
print("1. Sales Amount Distribution")
print("2. Sales by Region")
print("3. Sales by Product Category")
print("4. Sales by Sales Representative")
print("5. Quantity Sold Distribution")
print("6. Sales Channel Analysis")

choice = input("👉 Enter your choice: ")

if choice == "1":
    df["Sales_Amount"].plot(kind="hist", bins=20, title="📊 Sales Amount Distribution")
    plt.xlabel("Sales Amount")
    plt.show()

elif choice == "2":
    df.groupby("Region")["Sales_Amount"].sum().plot(
        kind="bar", title="🌍 Total Sales by Region"
    )
    plt.xlabel("Region")
    plt.ylabel("Total Sales")
    plt.show()

elif choice == "3":
    df.groupby("Product_Category")["Sales_Amount"].sum().plot(
        kind="bar", title="🛍️ Total Sales by Product Category"
    )
    plt.xlabel("Product Category")
    plt.ylabel("Total Sales")
    plt.show()

elif choice == "4":
    df.groupby("Sales_Rep")["Sales_Amount"].sum().plot(
        kind="bar", title="👤 Total Sales by Sales Representative"
    )
    plt.xlabel("Sales Representative")
    plt.ylabel("Total Sales")
    plt.show()

elif choice == "5":
    df["Quantity_Sold"].plot(
        kind="hist", bins=15, title="📦 Quantity Sold Distribution"
    )
    plt.xlabel("Quantity Sold")
    plt.show()

elif choice == "6":
    df.groupby("Sales_Channel")["Sales_Amount"].sum().plot(
        kind="bar", title="🛒 Sales by Channel"
    )
    plt.xlabel("Sales Channel")
    plt.ylabel("Total Sales")
    plt.show()

else:
    print("❌ Invalid choice!")


    📈 == Data Visualization ==
1. Sales Amount Distribution
2. Sales by Region
3. Sales by Product Category
4. Sales by Sales Representative
5. Quantity Sold Distribution
6. Sales Channel Analysis
👉 Enter your choice: 2

📊 Graph displayed successfully!



# 💾 Step 7: Save Visualization

print("\n💾 == Save Visualization ==")
print("1. Save Sales Amount Distribution")
print("2. Save Sales by Region")
print("3. Save Sales by Product Category")
print("4. Save Sales by Sales Representative")

choice = input("👉 Enter your choice: ")

if choice == "1":
    df["Sales_Amount"].plot(kind="hist", bins=20, title="📊 Sales Amount Distribution")
    plt.xlabel("Sales Amount")
    plt.savefig("sales_amount_distribution.png")
    plt.show()
    print("✅ Visualization saved successfully!")

elif choice == "2":
    df.groupby("Region")["Sales_Amount"].sum().plot(
        kind="bar", title="🌍 Total Sales by Region"
    )
    plt.xlabel("Region")
    plt.ylabel("Total Sales")
    plt.savefig("sales_by_region.png")
    plt.show()
    print("✅ Visualization saved successfully!")

elif choice == "3":
    df.groupby("Product_Category")["Sales_Amount"].sum().plot(
        kind="bar", title="🛍️ Sales by Product Category"
    )
    plt.xlabel("Product Category")
    plt.ylabel("Total Sales")
    plt.savefig("sales_by_category.png")
    plt.show()
    print("✅ Visualization saved successfully!")

elif choice == "4":
    df.groupby("Sales_Rep")["Sales_Amount"].sum().plot(
        kind="bar", title="👤 Sales by Sales Representative"
    )
    plt.xlabel("Sales Representative")
    plt.ylabel("Total Sales")
    plt.savefig("sales_by_sales_rep.png")
    plt.show()
    print("✅ Visualization saved successfully!")

else:
    print("❌ Invalid choice!")


    💾 == Save Visualization ==
1. Save Sales Amount Distribution
2. Save Sales by Region
3. Save Sales by Product Category
4. Save Sales by Sales Representative
👉 Enter your choice: 2

📊 Graph displayed
💾 File saved as: sales_by_region.png
✅ Visualization saved successfully!


# 🚪 Step 8: Exit

print("\n🚪 == Exit ==")
print("👋 Thank you for using the Data Analysis & Visualization Project!")
print("✅ Program exited successfully.")

🚪 == Exit ==
👋 Thank you for using the Data Analysis & Visualization Project!
✅ Program exited successfully.




