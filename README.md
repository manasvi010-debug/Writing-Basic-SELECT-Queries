# Writing-Basic-SELECT-Queries
Writing Basic SELECT Queries
SELECT 
    first_name, 
    last_name, 
    department, 
    salary, 
    email
FROM employees
WHERE 
    -- must be in Sales or Engineering
    (department = 'Sales' OR department = 'Engineering')
    
    -- salary must be between 60k and 90k
    AND salary BETWEEN 60000 AND 90000
    
    -- email must end with example.com
    AND email LIKE '%@example.com'
ORDER BY 
    department ASC,   -- sort departments alphabetically
    salary DESC;      -- highest salaries first
