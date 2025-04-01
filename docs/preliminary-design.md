# Preliminary Design - Company Database

## Entities & Attributes
1. **Employee**
   - `ID` (Primary Key)
   - `Name` (Composite Attribute)
     - `Fname`
     - `Mname` (Optional)
     - `Lname`
   - `SSN`
   - `Sex`
   - `Address`
   - `Bdate`
   - `Phone_num`
   - `Salary`
   - `HireDate`
  
2. **Department**
   - `DepID` (Primary Key)
   - `DepName`
   - `Location`

## Relationships
- Employee **Works_for** Departments (1:N)
- Departments **Manages** Departments (1:1)  
- Employee **Supervision** Employee (1:N)
