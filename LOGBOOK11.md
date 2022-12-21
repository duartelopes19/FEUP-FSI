# Log Book 11

## Task 1

### What part of the certificate indicates this is a CA’s certificate?
![](imgs/week11/task1-1.png)

### What part of the certificate indicates this is a self-signed certificate?
The Issuer is the same as the Subject.
![](imgs/week11/task1-2.png)

### In the RSA algorithm, we have a public exponent e, a private exponent d, a modulus n, and two secret numbers p and q, such that n = pq. Please identify the values for these elements in your certificate and key files.

- Public exponent, e:

![](imgs/week11/task1-3.png)

- Private exponent, d:

![](imgs/week11/task1-5.png)

- Modulus, n:
  
![](imgs/week11/task1-4.png)

- To find the private key, we need to find the two secret numbers p and q, such that n=p*q:
  - p:
    ![](imgs/week11/task1-6.png)
  - q:
    ![](imgs/week11/task1-7.png) 

## Task 2
We generated the certificate signing request (CSR).

![](imgs/week11/task2.png)

## Task 3
We generated the certificate.

![](imgs/week11/task3-1.png)

Print of the decoded content of the
certificate:

![](imgs/week11/task3-2.png)

## Task 4
...

## Task 5
...

## Task 6
...

---

## CTF 11