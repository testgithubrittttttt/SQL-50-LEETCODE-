# Write your MySQL query statement below
SELECT 
    CASE 
        WHEN id = (SELECT MAX(id) FROM seat) AND id % 2 = 1
            THEN id 
        WHEN id % 2 = 1
            THEN id + 1
        ELSE id - 1
    END AS id,
    student
FROM seat
ORDER BY id
