# sieve-of-eratosthenes
Implementation of a program that computes prime numbers. One of the most basic ways to compute prime numbers is the Sieve of Eratosthenes. It's a simple algorithm that works as follows:

Suppose I want to find all prime numbers up to 100. Create an array with a location for every possible numbers from 0 to 100. In other words, create an array of size max+1. Then initialize that array to all true. Until we know otherwise, we will assume all numbers are prime. The Sieve of Eratosthenes works by removing the numbers that are not prime. What is left is the prime numbers.

Set the locations 0 and 1 to false (or just ignore them). Those are not primes by definition. Then, for every value from 2 to size/2, set all multiples greater than one of the value to false. For 2, we would set 4, 6, 8, 10, etc. to false, since we know they are not primes. For 3, we would set 6, 9, 12, etc. since we know they are not primes.

Whatever is left is a prime number.
