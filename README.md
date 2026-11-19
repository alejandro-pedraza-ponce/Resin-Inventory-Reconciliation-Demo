# Resin Inventory Reconciliation Demo

## Purpose

Automates the inventory adjustment process by comparing physical inventory to system inventory, identifying differences, determining the required movements, connecting those movements to production orders and work centers, and generating copy-ready entries for the final reports.

## Workflow

**Source Reports → Compare Physical to System Inventory → Identify Movements Needed → Select Orders & Assign Quantities → Match Work Centers → Generate Reports**

## Source Reports

The first four sheets contain data from separate operational reports: Physical Inventory, System Inventory, Production Orders, and Work Centers.

The first three reports provide the data needed to identify inventory differences and determine the required movement: Consumption or Reversal.

The Work Center Report is obtained after Order Allocation because the production orders must first be selected. Column H, **Orders Used**, in the Order Allocation sheet identifies the production orders actually used, allowing the Work Center Report to retrieve only the information needed for those specific orders rather than processing all available production data.

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

![Inventory Reconciliation](inventory-reconciliation.png)

### Order Allocation

![Order Allocation](order-allocation.png)

### Generated Report

![Generated Report](generated-report.png)

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
