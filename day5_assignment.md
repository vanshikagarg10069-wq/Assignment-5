QUESTION 1.
| Line No.    | Error                                                            | Error Type            | Correction                                        |
| ----------- | ---------------------------------------------------------------- | --------------------- | ------------------------------------------------- |
| 6           | Missing semicolon after `int marks[5] = {80,90,70,60,50}`        | Syntax Error          | `int marks[5] = {80,90,70,60,50};`                |
| 12          | `i <= 5` accesses `marks[5]` (out of bounds)                     | Runtime/Logical Error | `for(int i=0; i<5; i++)`                          |
| 21          | `printf("Average = %d\n", average);` uses wrong format specifier | Semantic Error        | `printf("Average = %.2f\n", average);`            |
| 32          | `scores[5] = 60;` exceeds array size                             | Runtime Error         | Remove statement or increase array size           |
| 45          | `strcpy(subject,"Programming");` overflows array `subject[5]`    | Runtime Error         | Increase size: `char subject[20];`                |
| 54          | `attendance["one"] = 1;` uses string as index                    | Syntax/Semantic Error | Use integer index, e.g., `attendance[1] = 1;`     |
| 56          | `attendance[2.5] = 1;` uses float index                          | Syntax/Semantic Error | Use integer index, e.g., `attendance[2] = 1;`     |
| 65          | `i <= 5` accesses `attendance[5]`                                | Runtime Error         | `for(int i=0; i<5; i++)`                          |
| 75          | `scanf("%d", arr[i]);` missing address operator                  | Runtime Error         | `scanf("%d", &arr[i]);`                           |
| 91          | `grade[0] = "A";` assigns string to char                         | Syntax Error          | `grade[0] = 'A';`                                 |
| 94          | `printf("%s\n", grade);` string may not be null terminated       | Runtime Error         | Add `grade[2] = '\0';` before printing            |
| 100         | `if(prices[2] = 300)` uses assignment instead of comparison      | Logical Error         | `if(prices[2] == 300)`                            |
| 109         | `inventory = prices;` array assignment not allowed               | Syntax Error          | Copy using loop or `memcpy()`                     |
| 118         | `printf("%d\n", salary[0]);` wrong format specifier for float    | Semantic Error        | `printf("%.2f\n", salary[0]);`                    |
| 124         | `city = "Jaipur";` array assignment not allowed                  | Syntax Error          | `strcpy(city, "Jaipur");`                         |
| 133         | `i <= 5` writes to `result[5]`                                   | Runtime Error         | `for(int i=0; i<5; i++)`                          |
| 20          | `average = total / 5;` performs integer division                 | Logical Error         | `average = (float)total / 5;`                     |
| 89          | `char grade[5];` not initialized before string print             | Runtime Error         | Initialize properly: `char grade[5] = "A+";`      |
| 108         | `inventory[0]` used without valid initialization                 | Runtime Error         | Copy values from `prices` first                   |
| 123         | `city` declared but not initialized before assignment attempt    | Semantic Error        | Use `strcpy(city, "Jaipur");`                     |
| Entire File | Same program repeated multiple times                             | Syntax Error          | Keep only one complete program in the source file |

QUESTION 2.
| Line No. | Error                                                                 | Error Type                          | Correction                                  |
| -------- | --------------------------------------------------------------------- | ----------------------------------- | ------------------------------------------- |
| 15       | `for(int i=0;i<=10;i++)` accesses `numbers[10]`                       | Runtime Error (Array Out of Bounds) | `for(int i=0;i<10;i++)`                     |
| 25       | `sum = numbers[i];` only stores last value instead of adding          | Logical Error                       | `sum += numbers[i];`                        |
| 33       | `printf("Average = %d\n", average);` wrong format specifier for float | Semantic Error                      | `printf("Average = %.2f\n", average);`      |
| 31       | `average = sum / 10;` performs integer division                       | Logical Error                       | `average = (float)sum / 10;`                |
| 44       | `if(marks[i] < highest)` finds minimum instead of highest             | Logical Error                       | `if(marks[i] > highest)`                    |
| 60       | `attendance[5] = 1;` exceeds array size                               | Runtime Error                       | Remove statement or increase array size     |
| 64       | `for(int i=0;i<=5;i++)` accesses `attendance[5]`                      | Runtime Error                       | `for(int i=0;i<5;i++)`                      |
| 74       | `strcpy(subject,"ComputerScience");` string larger than array size 10 | Runtime Error                       | Increase array size: `char subject[20];`    |
| 82       | `branch = "IT";` array assignment not allowed                         | Syntax Error                        | `strcpy(branch,"IT");`                      |
| 96       | `printf("%s\n", college);` string not null terminated                 | Runtime Error                       | Add `college[5] = '\0';`                    |
| 102      | `fees["two"] = 50000;` string used as array index                     | Syntax/Semantic Error               | Use integer index, e.g., `fees[2] = 50000;` |
| 104      | `fees[3.5] = 60000;` float used as array index                        | Syntax/Semantic Error               | Use integer index, e.g., `fees[3] = 60000;` |
| 122      | `scanf("%d", result[i]);` missing address operator                    | Runtime Error                       | `scanf("%d", &result[i]);`                  |
| 139      | `if(stock[2] = 300)` assignment instead of comparison                 | Logical Error                       | `if(stock[2] == 300)`                       |
| 148      | `backup = stock;` array assignment not allowed                        | Syntax Error                        | Copy using loop or `memcpy()`               |
| 157      | `printf("%d\n", salary[0]);` wrong format specifier for float         | Semantic Error                      | `printf("%.2f\n", salary[0]);`              |
| 163      | `for(int i=0;i<=5;i++)` accesses `inventory[5]`                       | Runtime Error                       | `for(int i=0;i<5;i++)`                      |
| 177      | `strcpy(city,"JaipurCity");` string exceeds array size 8              | Runtime Error                       | Increase size: `char city[11];`             |
| 185      | `count = inventory;` array assignment not allowed                     | Syntax Error                        | Copy elements using loop                    |
| 191      | Missing semicolon after `printf("Program Ended\n")`                   | Syntax Error                        | `printf("Program Ended\n");`                |

QUESTION 3.
| Line No.    | Error                                                         | Error Type            | Correction                              |
| ----------- | ------------------------------------------------------------- | --------------------- | --------------------------------------- |
| 19          | `average = total / 5;` performs integer division              | Logical Error         | `average = (float)total / 5;`           |
| 40          | `if(marks[i] > lowest)` finds highest instead of lowest       | Logical Error         | `if(marks[i] < lowest)`                 |
| 58          | `for(int i=0;i<=5;i++)` accesses `attendance[5]`              | Runtime Error         | `for(int i=0;i<5;i++)`                  |
| 68          | `char subject[8];` too small for `"Programming"`              | Runtime Error         | `char subject[12];` (or larger)         |
| 70          | `strcpy(subject,"Programming");` causes buffer overflow       | Runtime Error         | Increase array size before copying      |
| 78          | `scanf("%s",&branch);` incorrect argument                     | Semantic Error        | `scanf("%9s", branch);`                 |
| 91          | `fees[5] = 100000;` exceeds array size                        | Runtime Error         | Remove statement or increase array size |
| 103         | `if(stock[2] = 30)` uses assignment instead of comparison     | Logical Error         | `if(stock[2] == 30)`                    |
| 112         | `backup = stock;` array assignment not allowed                | Syntax Error          | Copy elements using loop or `memcpy()`  |
| 121         | `printf("%d\n", salary[0]);` wrong format specifier for float | Semantic Error        | `printf("%.2f\n", salary[0]);`          |
| 129         | `scanf("%d", result[i]);` missing address operator            | Runtime Error         | `scanf("%d", &result[i]);`              |
| 145         | `city = "Jaipur";` array assignment not allowed               | Syntax Error          | `strcpy(city, "Jaipur");`               |
| 153         | `inventory["one"] = 100;` string used as array index          | Syntax/Semantic Error | `inventory[1] = 100;`                   |
| 155         | `inventory[2.5] = 200;` float used as array index             | Syntax/Semantic Error | `inventory[2] = 200;`                   |
| 165         | `for(int i=0;i<=5;i++)` accesses `inventory[5]`               | Runtime Error         | `for(int i=0;i<5;i++)`                  |
| 177         | `char college[5];` no space for null terminator               | Runtime Error         | `char college[6];`                      |
| 184         | `printf("%s\n", college);` string not null terminated         | Runtime Error         | Add `college[5] = '\0';`                |
| 190         | `count = inventory;` array assignment not allowed             | Syntax Error          | Copy values using loop                  |
| 198         | `char course[6];` too small for `"Computer"`                  | Runtime Error         | `char course[9];`                       |
| 200         | `strcpy(course,"Computer");` causes buffer overflow           | Runtime Error         | Increase array size                     |
| 208         | `for(int i=0;i<=5;i++)` accesses `numbers[5]`                 | Runtime Error         | `for(int i=0;i<5;i++)`                  |
| 220         | Missing semicolon after `return 0`                            | Syntax Error          | `return 0;`                             |
| Entire File | Program repeated multiple times in same source file           | Syntax Error          | Keep only one complete program          |

QUESTION 4.
| Line No. | Error                                           | Error Type                          | Error Correction                                                      |
| -------- | ----------------------------------------------- | ----------------------------------- | --------------------------------------------------------------------- |
| 20       | `printf("Average Sales = %d\n", averageSales);` | Semantic Error                      | Use `%f` for float: `printf("Average Sales = %.2f\n", averageSales);` |
| 28       | `if(sales[i] < highestSale)`                    | Logical Error                       | Use `>` to find highest sale: `if(sales[i] > highestSale)`            |
| 45       | `monthlySales[5] = 250;`                        | Runtime Error (Array Out of Bounds) | Use valid index (0–4) or increase array size.                         |
| 50       | `for(int i=0;i<=5;i++)`                         | Runtime Error                       | Change to `for(int i=0;i<5;i++)`                                      |
| 60       | `char product[8];` with `"LaptopComputer"`      | Runtime Error (Buffer Overflow)     | Increase size: `char product[20];`                                    |
| 70       | `category = "Electronics";`                     | Syntax Error                        | Use `strcpy(category, "Electronics");`                                |
| 78       | `stock["first"] = 100;`                         | Syntax Error                        | Use integer index: `stock[0] = 100;`                                  |
| 80       | `stock[2.7] = 200;`                             | Syntax Error                        | Use integer index: `stock[2] = 200;`                                  |
| 101      | `scanf("%d", orders[i]);`                       | Runtime Error                       | Pass address: `scanf("%d", &orders[i]);`                              |
| 118      | `if(revenue[2] = 3000)`                         | Logical Error                       | Use comparison operator: `if(revenue[2] == 3000)`                     |
| 127      | `backupRevenue = revenue;`                      | Syntax Error                        | Copy elements using loop or `memcpy()`.                               |
| 135      | `printf("%d\n", commission[0]);`                | Semantic Error                      | Use `%f`: `printf("%f\n", commission[0]);`                            |
| 141      | `city = "Jaipur";`                              | Syntax Error                        | Use `strcpy(city, "Jaipur");`                                         |
| 152      | `printf("%s\n", branch);`                       | Runtime Error                       | Add null terminator: `branch[4] = '\0';`                              |
| 160      | `for(int i=0;i<=5;i++)`                         | Runtime Error                       | Change to `for(int i=0;i<5;i++)`                                      |
| 176      | `char department[6];` with `"Marketing"`        | Runtime Error (Buffer Overflow)     | Increase size: `char department[10];` or larger.                      |
| 184      | `expenses = sales;`                             | Syntax Error                        | Copy array elements using loop or `memcpy()`.                         |
| 192      | `ratings[-1] = 5;`                              | Runtime Error (Invalid Index)       | Use valid index: `ratings[0] = 5;`                                    |
| 204      | `printf("%s\n", feedback[0]);`                  | Semantic Error                      | Use `%d`: `printf("%d\n", feedback[0]);`                              |
| 208      | `printf("Report Generated Successfully\n")`     | Syntax Error                        | Add semicolon: `printf("Report Generated Successfully\n");`           |

QUESTION 5.
| Line No. | Error                                       | Error Type                          | Error Correction                                                 |
| -------- | ------------------------------------------- | ----------------------------------- | ---------------------------------------------------------------- |
| 20       | `printf("Average = %d\n", average);`        | Semantic Error                      | Use `%f` for float: `printf("Average = %.2f\n", average);`       |
| 28       | `if(marks[i] < highest)`                    | Logical Error                       | Use `>` to find highest mark: `if(marks[i] > highest)`           |
| 40       | `if(marks[i] > lowest)`                     | Logical Error                       | Use `<` to find lowest mark: `if(marks[i] < lowest)`             |
| 56       | `attendance[10] = 0;`                       | Runtime Error (Array Out of Bounds) | Valid indices are 0–9. Use a valid index or increase array size. |
| 60       | `for(int i=0;i<=10;i++)`                    | Runtime Error                       | Change to `for(int i=0;i<10;i++)`                                |
| 70       | `char subject[10];` with `"DataStructures"` | Runtime Error (Buffer Overflow)     | Increase size: `char subject[15];` or larger.                    |
| 78       | `department = "InformationTechnology";`     | Syntax Error                        | Use `strcpy(department, "InformationTechnology");`               |
| 86       | `fees["two"] = 50000;`                      | Syntax Error                        | Use integer index: `fees[2] = 50000;`                            |
| 88       | `fees[4.5] = 70000;`                        | Syntax Error                        | Use integer index: `fees[4] = 70000;`                            |
| 109      | `scanf("%d", result[i]);`                   | Runtime Error                       | Pass address: `scanf("%d", &result[i]);`                         |
| 126      | `if(inventory[2] = 30)`                     | Logical Error                       | Use comparison operator: `if(inventory[2] == 30)`                |
| 135      | `backup = inventory;`                       | Syntax Error                        | Copy array elements using a loop or `memcpy()`.                  |
| 143      | `printf("%d\n", salary[0]);`                | Semantic Error                      | Use `%f`: `printf("%f\n", salary[0]);`                           |
| 149      | `city = "Jaipur";`                          | Syntax Error                        | Use `strcpy(city, "Jaipur");`                                    |
| 160      | `printf("%s\n", branch);`                   | Runtime Error                       | Add null terminator: `branch[4] = '\0';`                         |
| 168      | `for(int i=0;i<=5;i++)`                     | Runtime Error                       | Change to `for(int i=0;i<5;i++)`                                 |
| 184      | `char course[8];` with `"Programming"`      | Runtime Error (Buffer Overflow)     | Increase size: `char course[12];` or larger.                     |
| 194      | `ratings[-1] = 10;`                         | Runtime Error (Invalid Index)       | Use a valid index such as `ratings[0] = 10;`                     |
| 200      | `printf("%s\n", feedback[0]);`              | Semantic Error                      | Use `%d`: `printf("%d\n", feedback[0]);`                         |
| 208      | `scores = marks;`                           | Syntax Error                        | Copy array elements using a loop or `memcpy()`.                  |
| 220      | `printf("%d\n", temp[5]);`                  | Runtime Error (Array Out of Bounds) | Use a valid index (0–4).                                         |
