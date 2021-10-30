# dsa
concept and implementation using java

# Hashing:
 - It is used for fast retrival and store value.

Hashing Technics for resolve collision(टक्कर):
1. Division
2. Folding 
3. Mid Squre
4. Moduler multiplication

Search Technics:
1. Linear Search - O(n)
2. Binary Search - O(log n)

Open Addressing - Chaining Method

Chaining Method:
   - (If collision happens then compare exsting value and build chain example: Hashmap - Array-Of-LinkedList)
https://www.youtube.com/watch?v=zeMa9sg-VJM

Close Addressing - Linear Probling, Quarditic Probling, Double Probling Method
 - Linear Probling: 
   - (If collision happens then find next available location and insert element)
https://www.youtube.com/watch?v=zeMa9sg-VJM
   - Steps:
   - 1. key = 5, m = 10; where m is maxBucketSize.
   - Calculate Hash value of key hash(key) = key % m; hash(5) = 5%10;
   - run loop to find available local from hash-calculated for i = 0..10 increse i++ { arr[(hash(5)+i)%m] == null -> insert(5); break;}
Quarditic Probling:
https://www.youtube.com/watch?v=dxrLtf-Fybk
   - Steps:
   - 1. key = 5, m = 10; where m is maxBucketSize.
   - Calculate Hash value of key hash(key) = key % m; hash(5) = 5%10;
   - run loop to find available local from hash-calculated for i = 0..10 increse i++ { arr[(hash(5)+(i power 2))%m] == null -> insert(5); break;}
Double Hashing:
https://www.youtube.com/watch?v=AYcsTOeFVas
   - for i = 0..10 increse i++ { arr[(hash(5)+ (V*i))%m] == null -> insert(5); break;}
