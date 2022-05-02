# Pewlett_Hackard_Analysis

# Project Overview
The business client Pewlett Hackard has an influx of retirements incoming. The task required analyzing databases to determine the number of employees retiring and the number eligible employees for mentorship. With this information, the client can make accurate hiring decisions.


## Resources

[W3 - Natural Join](https://www.w3resource.com/sql/joins/natural-join.php)

[PostgreSQL - Distinct Clause](https://www.postgresql.org/docs/9.5/sql-select.html)

# Results



## Retiring Employees

### Retiring Departments

    SELECT COUNT(den.emp_no),
    den.dept_name
    INTO dept_retiring
    FROM dept_emp_no as den
    INNER JOIN retirement_info as ri
    ON (den.emp_no = ri.emp_no)
    GROUP BY den.dept_name
    ORDER BY COUNT(den.emp_no) DESC;
## Mentorship Eligibility




# Summary

