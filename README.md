# Q.25
# Example matrices
matrix1 = [[1, 2, 3],
           [4, 5, 6],
           [7, 8, 9]]
matrix2 = [[10, 11, 12],
           [13, 14, 15],
           [16, 17, 18]]

# Initialize result matrix with zeros
result = [[0 for _ in range(len(matrix2[0]))] for _ in range(len(matrix1))]

# Perform matrix multiplication
for i in range(len(matrix1)):
    for j in range(len(matrix2[0])):
        for k in range(len(matrix2)):
            result[i][j] += matrix1[i][k] * matrix2[k][j]

# Print the result matrix
for row in result:
    print(row)
