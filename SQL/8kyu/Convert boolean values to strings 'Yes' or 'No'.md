```SQL
SELECT bool,
CASE
    WHEN bool = true THEN 'Yes'
    WHEN bool = false THEN 'No'
    ELSE NULL
END AS res
FROM booltoword;
```