```SQL
SELECT str,
CASE
  WHEN LOWER(str) != REVERSE(LOWER(str)) THEN false
  ELSE true
END AS res
FROM ispalindrome
```