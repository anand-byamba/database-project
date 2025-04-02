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
   - `Number_of_employees` (Derived Attribute)
  
3. **Project**
   - `Proj_name` (Primary key)
   - `Proj_ID`
   - `Location`
  
4. **Dependent**
   - `Name` (Weak Entity)
   - `Gender`
   - `Birth_date`
   - `Relationship`

## Relationships
- Employee **Works_for** Departments (1:N)
- Employee **Manages** Departments (1:1)
   - `Start_date`
- Employee **Supervision** Employee (1:N)
- Employee **Works_on** Project (M:N)
   - `Hours`
- Employee **Dependents_of** Dependent (1:N)
- Department **Controls** Project (1:N)
