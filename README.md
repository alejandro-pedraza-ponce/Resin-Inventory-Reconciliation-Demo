# Resin Inventory Reconciliation Demo

## Purpose

Automates the inventory adjustment process by comparing physical inventory to system inventory, identifying differences, determining the required movements, connecting those movements to production orders and work centers, and generating copy-ready entries for the final reports.

## Workflow

**Source Reports → Compare Physical to System Inventory → Identify Movements Needed → Select Orders & Assign Quantities → Match Work Centers → Generate Reports**

## How to Use

1. Review the source report sheets.
2. Open **Inventory Reconciliation** to compare physical inventory to system inventory and identify differences.
3. The workbook determines whether a **Consumption, Reversal, or no movement** is required.
4. Open **Order Allocation** to select the production order(s) used for each movement and assign the appropriate quantities (lbs).
5. Use Column H, **Orders Used**, to obtain the Work Center Report for the selected production orders.
6. The selected production orders are matched to their work centers and used to generate copy-ready entries for the final reports.

## Automation Highlights

- Compares physical inventory to system inventory automatically.
- Identifies inventory differences requiring action.
- Determines the required inventory movement.
- Accounts for incoming material that may temporarily affect inventory differences.
- Connects materials to available production orders and work centers.
- Tracks quantities assigned and quantities remaining.
- Generates formatted, copy-ready entries for two final reports.

## Screenshots

### Inventory Reconciliation

![Inventory Reconciliation](Inventory%20Reconciliation.png)

### Order Allocation

![Order Allocation](Order%20Allocation.png)

### Generated Report

![Generated Report](Generated%20Report.png)

## Video Demo

[▶ Watch the Project Walkthrough](https://www.loom.com/share/d8f5c1e829e843fc99d595889ac4732c)

## Demo Workbook

The complete sanitized Excel demo is included in this repository:

**`Resin-Inventory-Reconciliation-Demo.xlsx`**

## Demo Data

All data in this workbook is synthetic and was created solely for demonstration purposes. No company, employee, customer, or production data is included.

## Color Guide

- 🟢 **Green** = Within ±5,000 lbs tolerance. No inventory movement required.
- 🟡 **Yellow** = Difference exceeds ±5,000 lbs. Inventory movement required.
- 🔴 **Red** = Incoming Material. No movement is required because the inventory difference may be temporary while material is being received.
- ⚫ **Gray** = N/A. Product is excluded from normal adjustment processing.

## Technologies Used

<div>
  <img src="https://img.icons8.com/color/1200/microsoft-excel-2019--v1.jpg" title="Microsoft Excel" alt="Microsoft Excel" width="60" height="60">&nbsp;&nbsp;
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSQ-Xo6QRq6JjoFXRlWyotLzm-BkxQFxcmlxC8x-ckhQA&s=10" title="Microsoft Copilot" alt="Microsoft Copilot" width="60" height="60">
</div>
