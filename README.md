# Resin Inventory Reconciliation Demo

An Excel-based workflow automation project designed to simplify a multi-step inventory adjustment process from the initial inventory comparison through final reporting.

## Why I Built It

This project started with a repetitive manual task: comparing physical inventory against system inventory and calculating the differences.

As I worked through the process, I realized there were additional repetitive steps that could also be automated, including determining required inventory movements, finding available production orders, tracking quantities, matching work centers, and preparing the final reports.

What started as automating one calculation gradually became a tool for automating most of the workflow.

## Workflow

**Source Reports → Compare Physical to System Inventory → Identify Movements Needed → Select Orders & Assign Quantities → Match Work Centers → Generate Reports**

## What It Does

- Compares physical inventory against system inventory automatically.
- Identifies inventory differences requiring action.
- Determines whether a Consumption, Reversal, or no movement is required.
- Uses a ±5,000 lb tolerance to prevent unnecessary movements.
- Accounts for incoming material that may temporarily affect inventory differences.
- Connects materials to available production orders.
- Allows the user to select the production orders actually used and assign quantities.
- Tracks quantities assigned and quantities remaining.
- Uses only the selected production orders to obtain the required work center information.
- Matches selected production orders to their corresponding work centers.
- Generates formatted, copy-ready entries for two final reports.

## Human Control

The workbook automates calculations and repetitive steps, but the user remains in control of important decisions such as selecting which production orders are actually used and how quantities are allocated between them.

## Video Demo

[▶ Watch the Project Walkthrough](https://www.loom.com/share/d8f5c1e829e843fc99d595889ac4732c)

## Demo Workbook

The repository includes the complete sanitized Excel workbook:

**`Resin-Inventory-Reconciliation-Demo.xlsx`**

Download the workbook to explore the workflow and formulas.

> **Note:** The workbook uses modern Excel functions and is intended for a current version of Microsoft Excel.

## Demo Data

All data in this workbook is synthetic and was created solely for demonstration purposes.

**No company, employee, customer, or production data is included.**

## Tools

- Microsoft Excel
- Dynamic Array Formulas
- LET
- FILTER
- XLOOKUP
- MAP
- SCAN
- REDUCE
- Conditional Formatting
- Data Validation

## Project Goal

The goal of this project was not simply to automate a calculation. It was to understand the entire workflow, identify repetitive manual steps, and create a solution that makes the process faster, more consistent, and easier to follow.
