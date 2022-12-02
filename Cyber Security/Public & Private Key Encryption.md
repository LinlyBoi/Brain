#CyberSecurity 

## Private key encryption
> Literally AES/DES
> Symmetric encryption 
> Same key for decryption and encryption
----
## Public Key encryption
> Asymmetric encryption
> Different keys for encryption and decryption
> More secure
> Sender can't decrypt the message sent 
----
### RSA
> Uses 2 prime large numbers ($p$, $q$)
> $n = p \cdot q$
> totient is calulated ($\phi$)
> $\phi{(n)} = (p-1)(q-1)$
> encryption number ($e$) is a coprime number to totient of n
> coprime $\rightarrow$ highest common divisor is 1 (e mod n = 1)
> decryption number $\rightarrow$ $d$ (private)
> $d \cdot e = 1 \mod \phi{(n)}$
> $d \cdot e = 1 + (k \cdot \phi{(n)})$ 
> Encryption $\rightarrow$ $C = M^e \mod \space n$
> Decryption $\rightarrow$ $M = C^d \mod n$
> Public key $\rightarrow$ $\{e, n\}$ 
> Private key $\rightarrow$ $\{d, n\}$
----
## Diffe-Helman
> Requires $q$ and $\alpha$
> $q$ is a large prime number
> $\alpha$ is an integer
> $X_a$ and $X_b$ are chosen where they are random numbers less than $q$
>$Y_a = \alpha^{X_a} \mod q$
>$Yb = \alpha^{X_b} \mod q$
>$Y_b$ and $Y_a$ are exchanged
>$K = {Y_a}^{X_b} = {Y_b}^{X_a}$
>$\alpha$ and $q$ are agreed upon, $X_a$ and $X_b$ are private, $Y_a$ and $Y_b$ are exchanged to get the key
>Can be used to generate AES keys
