# 📊 Using SUMIF & UNIQUE to Find Top-Selling Products in Excel

This repository contains resources for my YouTube tutorial:  
📺 https://youtu.be/opaZPhYLvfw

In this data analytics project, I demonstrate how to use Excel’s **SUMIF** and **UNIQUE** functions to analyze sales data and automatically identify the **top-selling product**.  
It’s a beginner-friendly approach to basic data analytics using only formulas — no PivotTables required.

---

## 📂 Repository Contents
- `IceCreamSales.xlsx` → Sample dataset with weeks, flavors, and units sold  
- `README.md` → Documentation explaining the method  
---

## 🧮 Step-by-Step Guide

### 1. Extract Unique Products
To get a list of all distinct flavors (without duplicates), inside the E2 cell use:

```excel
=UNIQUE(C2:C100)
````

This scans the **Flavor** column and generates a clean list of unique items.

---

### 2. Calculate Total Sales per Product

Once we have unique products, we can calculate their total sales using **SUMIF**:

```excel
=SUMIF(C:C, E2, B:B)
```
**Explanation:**

* **C:C** → Flavor column
* **E2** → A single unique flavor (like "Chocolate")
* **B:B** → Units sold column
* [Write the function into the F2 cell]

Dragging this formula down gives totals for all flavors automatically.

---

### 3. Identify the Top-Selling Product

Now, simply look for the **highest total sales value** in the results.
That product is your **best seller**, which can be recommended to management for decisions like production, marketing, or promotions.

---

## 🔗 Related Resources

* 📺 [SUMIF & UNIQUE Tutorial Video](https://youtu.be/opaZPhYLvfw)
* 📺 [🔥Excel VLOOKUP Made Easy | Learn with Dynamic Tables + Free Practice File](https://youtu.be/IYg_m0PTYPk)
* 📂 [Download Sample Excel Sheet](https://github.com/Kami2021/excel-sumif-unique-top-selling-products/blob/main/IceCreamSales.xlsx)

---

## 🙌 Support

If you found this project helpful:

* ⭐ Star this repository on GitHub
* 👍 Like the YouTube video
* 🔔 Subscribe for more Excel tutorials




