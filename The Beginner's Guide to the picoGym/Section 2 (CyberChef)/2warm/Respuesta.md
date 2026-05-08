Para convertir **42 decimal** a **binario**, se divide entre **2** y se guardan los residuos:

```text
42 ÷ 2 = 21 residuo 0
21 ÷ 2 = 10 residuo 1
10 ÷ 2 = 5  residuo 0
5 ÷ 2  = 2  residuo 1
2 ÷ 2  = 1  residuo 0
1 ÷ 2  = 0  residuo 1
```

Ahora lees los residuos **de abajo hacia arriba**:

```text
1 0 1 0 1 0
```

Entonces:

```text
42₁₀ = 101010₂
```

Para picoCTF sería:

```text
picoCTF{101010}
```
