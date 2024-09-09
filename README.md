
# WavexProject

In this project, I created Sales and HR reports based on a dataset using Power BI.

## Table of Contents
1. [Sales Report](#sales-report)
2. [HR Report](#hr-report)
3. [Step 1 - Data Discovery](#step-1---data-discovery)
   - [A. Gathering Relevant Data](#a-gathering-relevant-data)
   - [B. Project-Specific Requirements](#b-project-specific-requirements)
4. [Step 2 - Import Data](#step-2---import-data)
5. [Step 3 - Data Transformation](#step-3---data-transformation)
   - [1. Rename Tables](#1-rename-tables)
   - [2. Remove Top Rows](#2-remove-top-rows)
   - [3. Remove Bottom Rows](#3-remove-bottom-rows)
   - [4. Use First Row as Header](#4-use-first-row-as-header)
   - [5. Rename Columns](#5-rename-columns)
   - [6. Unpivot Columns](#6-unpivot-columns)
     - [A1. Unpivot Category Table](#a1-unpivot-category-table)
     - [B1. Unpivot ProductName Table](#b1-unpivot-productname-table)
   - [7. Column Quality](#7-column-quality)
   - [8. Remove Blank Rows](#8-remove-blank-rows)
   - [9. Remove Duplicates](#9-remove-duplicates)
   - [10. Append Queries](#10-append-queries)
   - [11. Choose Columns](#11-choose-columns)
   - [12. Merge Queries](#12-merge-queries)
   - [13. Clean (Format)](#13-clean-format)
   - [14. Split Column](#14-split-column)
     - [A1. Split by Delimiter](#a1-split-by-delimiter)
     - [A2. Rename New Columns](#a2-rename-new-columns)
     - [B1. Split by Number of Characters](#b1-split-by-number-of-characters)
     - [B2. Rename New Columns](#b2-rename-new-columns)
     - [B3. Hide Old Columns](#b3-hide-old-columns)
   - [15. Trim](#15-trim)
   - [16. Replace Values](#16-replace-values)
     - [A. Replace values in Country Column](#a-replace-values-in-country-column)
     - [B. Replace values in City Column](#b-replace-values-in-city-column)
   - [17. Capitalize Each Word](#17-capitalize-each-word)
   - [18. Merge Columns](#18-merge-columns)
   - [19. Extract](#19-extract)
     - [A. Extract Text Before Delimiter](#a-extract-text-before-delimiter)
     - [B. Extract Text After Delimiter](#b-extract-text-after-delimiter)
6. [Step 4 - Data Modeling and DAX](#step-4---data-modeling-and-dax)
7. [Step 5 - Creating Visualizations & Reports](#step-5---creating-visualizations--reports)

## Sales Report
![Sales Report](https://github.com/user-attachments/assets/f81fc73f-f124-4d74-962f-a94903f2cde7)

## HR Report
![HR Report](https://github.com/user-attachments/assets/84f7bb44-62ce-4ece-961e-39d4c684a78c)

## Step 1 - Data Discovery

### A. Gathering Relevant Data
- **Project**: WaveX Watercraft Company
- **Company Business**: Manufacturers of Jet Skis / Watercrafts
- **Data Provided**:
  - WaveX Company 2022 Sales Data (Text File)
  - WaveX Company Data (Excel)
  - WaveX Company Distributor List (PDF)

### B. Project-Specific Requirements
- Create two Power BI reports: Sales Report & HR Report
  1. Exclude data from 2018
  2. Exclude sales data from discontinued product WR3
  3. Create a sales forecast for the next two years

## Step 2 - Import Data
[Details on importing data]

## Step 3 - Data Transformation
This section outlines all the steps involved in the Data Transformation phase of this project.

### 1. Rename Tables
[Details on renaming tables]

### 2. Remove Top Rows
[Details on removing top rows]

### 3. Remove Bottom Rows
[Details on removing bottom rows]

### 4. Use First Row as Header
[Details on using the first row as a header]

### 5. Rename Columns
[Details on renaming columns]

### 6. Unpivot Columns
#### A1. Unpivot Category Table
[Details on unpivoting the category table]

#### B1. Unpivot ProductName Table
[Details on unpivoting the ProductName table]

### 7. Column Quality
[Details on checking column quality]

### 8. Remove Blank Rows
[Details on removing blank rows]

### 9. Remove Duplicates
[Details on removing duplicates]

### 10. Append Queries
[Details on appending queries]

### 11. Choose Columns
[Details on choosing columns]

### 12. Merge Queries
[Details on merging queries]

### 13. Clean (Format)
[Details on cleaning and formatting data]

### 14. Split Column
#### A1. Split by Delimiter
[Details on splitting columns by delimiter]

#### A2. Rename New Columns
[Details on renaming new columns]

#### B1. Split by Number of Characters
[Details on splitting columns by number of characters]

#### B2. Rename New Columns
[Details on renaming new columns]

#### B3. Hide Old Columns
[Details on hiding old columns]

### 15. Trim
[Details on trimming data]

### 16. Replace Values
#### A. Replace values in Country Column
- Replace “US” with “United States” and “UK” with “United Kingdom” in the Country column.

#### B. Replace values in City Column
[Details on replacing values in the City column]

### 17. Capitalize Each Word
- Capitalize each word in the “City” column.

### 18. Merge Columns
- Merge “DistributorFirstName” and “DistributorLastName” into a “FullName” column.

### 19. Extract
#### A. Extract Text Before Delimiter
- Extract text before “@” from the DistributorEmail column.

#### B. Extract Text After Delimiter
- Extract text after “@” from the DistributorEmail column.

## Step 4 - Data Modeling and DAX
In this section, I created my calculated measures to be used in the visualizations.
- **Example**: `TotalEmployees = COUNTROWS(HR)`
- **Example**: `TotalProductionCostColumn = Sales[CostPerUnit($)]*Sales[QuantitySold]`

## Step 5 - Creating Visualizations & Reports
[Details on creating visualizations and reports]
