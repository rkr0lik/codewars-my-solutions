```SQL
SELECT 
  name, 
  SUM(f.won) AS won, 
  SUM(f.lost) AS lost
FROM fighters f
    INNER JOIN winning_moves wm
        ON f.move_id = wm.id
WHERE wm.move NOT IN('Hadoken', 'Shouoken', 'Kikoken')
GROUP BY 
  name
ORDER BY 
  won DESC,
  lost DESC
LIMIT 6;
```