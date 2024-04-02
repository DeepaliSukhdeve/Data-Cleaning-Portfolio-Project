# Data-Cleaning-Portfolio-Project
Cleaning Data with SQL Queries






```

--Preview Data

Select *
From PortfolioProject.dbo.NashvilleHousing


```

```

-- Standardize Date Format


Select saleDate, CONVERT(Date,SaleDate)
From PortfolioProject.dbo.NashvilleHousing

ALTER TABLE NashvilleHousing
Add SaleDateConverted Date;

Update NashvilleHousing
SET SaleDateConverted = CONVERT(Date,SaleDate)


```
