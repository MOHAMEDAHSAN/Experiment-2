### Name : S Mohamed Ahsan
### Reg No : 212223240089

# Experiment-2
Write a program in Python language for Matrix multiplication fails. Introspect the causes for its failure and write down the possible reasons for its failure. 

## Aim
Write a python program for matrix multiplication and inspect for failures. 

## Algorithm
1.	Start the program.
2. Create empty list formatrix1, matrix2 and result.
3. Get the rows and columns count from the user.
4. Get the values of two matrix.
5. Perform matrix multiplication and store the answer in result.
6. Stop the program. 

## Program
print("Enter rows and columns for first matrix:")
r1, c1 = map(int, input().split())
print("Enter rows and columns for second matrix:")
r2, c2 = map(int, input().split())

if c1 != r2:
    print("Error")
else:
    m1 = [list(map(int, input().split())) for _ in range(r1)]
    m2 = [list(map(int, input().split())) for _ in range(r2)]
    res = [[0]*c2 for _ in range(r1)]
    for i in range(r1):
        for j in range(c2):
            for k in range(c1):
                res[i][j] += m1[i][k] * m2[k][j]
    print("Resultant Matrix:")
    for row in res:
        print(*row)

## Output
<img width="569" height="296" alt="image" src="https://github.com/user-attachments/assets/f6ab16cc-8dfe-4665-83ad-4a8103ba44cd" />

## Result
The multiplication of the given two matrices has been successfully performed.
The resultant matrix obtained is displayed above as the final output.
