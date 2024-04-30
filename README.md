# Prime number
Reference https://en.wikipedia.org/wiki/Prime_number
## Concepts
- A prime number is a natural number greater than 1 that is not a product of two smaller natural numbers.
- A natural number greater than 1 that is not prime is called a composite number
- If `i` is factor of `n` then `n/i` is also a factor of `n`. I.e. factors make a pair `(i, n/i)`. Therefore need to check between `1` to `sqrt(n)` 
- Every natural number greater than 1 is either a prime itself or can be factorized as a product of primes that is unique up to their order.
- primality test
    - Tests whether `n` is a multiple of any integer between `2` and `sqrt(n)`.
## Finding Prime numbers - Sieve of Eratosthenes
https://www.youtube.com/watch?v=eKp56OLhoQs
- Create list of all numbers from 2 to n
- Initially call all are prime
- Iterate each number from prime list
    - if prime[i] is prime then all multiples of prime[i] can't be prime
- Count rest of prime number
## Find GCD of two numbers?

## Find LCM of two numbers?
```
a * b = LCM(a,b) * GCD(a,b)
```

## How to store line slope in hash?
- Do not use y2-y1/x2-x1 as hash key
- main reason is fraction doesn't maintian accuracy 
- Use co-prime integers to represent unique slope
    - As a reminder, two integers are co-primes, if and only if their greatest common divisor is 1.
    ```
        const y = y2 - y1;
        const x = x2 - x1;
        if(x === 0) {
            return +Inf;
        }
        const d = gcd(x, y);
        return `${y/d}-${x/d}`;
    ``` 
## Mod

## Problems
https://leetcode.com/problems/count-primes/

https://www.lintcode.com/problem/kth-prime-number/description

https://leetcode.com/problems/the-kth-factor-of-n/

https://leetcode.com/problems/prime-palindrome/

https://leetcode.com/problems/k-th-smallest-prime-fraction/

https://leetcode.com/problems/prime-arrangements/

https://leetcode.com/problems/ugly-number/

https://leetcode.com/problems/ugly-number-ii/

https://leetcode.com/problems/ugly-number-iii/

https://leetcode.com/problems/super-ugly-number/

https://leetcode.com/problems/happy-number/

https://leetcode.com/problems/consecutive-numbers-sum/

https://leetcode.com/problems/mirror-reflection/

https://leetcode.com/tag/math/

https://leetcode.com/problems/best-meeting-point/

https://leetcode.com/problems/orderly-queue/

https://leetcode.com/problems/orderly-queue/

https://leetcode.com/problems/add-strings/

https://leetcode.com/problems/multiply-strings/

https://leetcode.com/problems/next-closest-time/
