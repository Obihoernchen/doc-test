# Subdir test

## Some random code

```bash
for dev in sdc sdd; do
  parted /dev/$dev mklabel gpt
  parted -a optimal /dev/$dev mkpart install 0% 500G
  parted -a optimal /dev/$dev mkpart misc 500G 1599G
  parted /dev/$dev set 1 raid on
  parted /dev/$dev set 2 raid on
done
```

## Some table

| Type                         | Name                     | Version        |
| ---------------------------- | ------------------------ | -------------- |
| Operating System             | Red Hat Enterprise Linux | 8.0            |
| System Management            | xCAT                     | 2.16.0         |
| InfiniBand                   | Mellanox OFED            | 4.7-1.0.0.1    |

!!! note
    Note test

!!! danger
    very dangerous

### Some more code

```python
# Program to display the Fibonacci sequence up to n-th term

nterms = int(input("How many terms? "))

# first two terms
n1, n2 = 0, 1
count = 0

# check if the number of terms is valid
if nterms <= 0:
   print("Please enter a positive integer")
# if there is only one term, return n1
elif nterms == 1:
   print("Fibonacci sequence upto",nterms,":")
   print(n1)
# generate fibonacci sequence
else:
   print("Fibonacci sequence:")
   while count < nterms:
       print(n1)
       nth = n1 + n2
       # update values
       n1 = n2
       n2 = nth
       count += 1
```
