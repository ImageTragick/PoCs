# ImageTragick POCs

## How To Use
```
git clone git@github.com:ImageTragick/PoCs.git
cd POCs
./test.sh
```

To test a `policy.xml` file place it in the script directory and run `test.sh`.

## Safe Output
```
user@host:~/code/PoCs$ ./test.sh 
testing read
SAFE

testing delete
SAFE

testing http with nonce: a7DyBeV7
SAFE

testing rce1
SAFE

testing rce2
SAFE

testing MSL
SAFE
```

## Unsafe Output
```
user@host:~/code/PoCs$ ./test.sh 
testing read
UNSAFE

testing delete
UNSAFE

testing http with nonce: a7DvBer2
UNSAFE

testing rce1
UNSAFE

testing rce2
UNSAFE

testing MSL
UNSAFE
```