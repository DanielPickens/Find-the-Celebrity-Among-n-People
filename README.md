# Find-the-Celebrity-Among-n-People
A game which computes the finding of a  celebrity amongst n people


My solution steps when writing my code: 

1. This program is utilizing a matrix such that matrix[i][j] is True if i person actuallky knows j person in real life.
2. Created two functions which well named variables: eliminate_non_celebrities and check_if_celebrity.
3. The function eliminate_non_celebrities returns a candidate who is maybe a celebrity. It takes the matrix as its  argument to do so.
4. The function check_if_celebrity determines whether a person is a celebrity. this function is used to  takes the matrix and the possible celebrity as argument to achieve/ find this out.
5. The function : eliminate_non_celebrities works on the principle that if matrix[i][j] = True, that is i knows j, then i cannot be the celebrity and if matrix[i][j] = False, that is i doesn’t know j, then j cannot be the celebrity.
6. The function check_if_celebrity checks whether possible_celeb is known by everyone else and whether possible_celeb doesn’t know anyone. If so, it then returns True = which is the celebrity. 



RUNTIME TEST CASES/UAT: 
Case 1:
Number of people: 6
Enter list of people known to 0: 3 2 0
Enter list of people known to 1: 1 0 2 3
Enter list of people known to 2: 4 1 3
Enter list of people known to 3: 
Enter list of people known to 4: 0 1 2 3 4 5
Enter list of people known to 5: 3
3 is the celebrity.


