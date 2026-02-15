```SQL
SELECT n,
CASE 
  WHEN ((n - 1) % 88 ) % 12  IN (1, 4, 6, 9, 11) THEN 'black'
  ELSE 'white'
END AS res
FROM pianokeys
```