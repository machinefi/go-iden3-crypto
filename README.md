## go-iden3-crypto
fork from [go-iden3-crypto](https://github.com/iden3/go-iden3-crypto)

## example

```go
	hexString := "470Eb48290776c370ffAd6224364a604AedfE7B9"
	bigInt := new(big.Int)
	bigInt.SetString(hexString, 16)
	b1 := big.NewInt(1)
	b2 := bigInt
	b3 := big.NewInt(2)
	b4 := big.NewInt(3)
	b5 := big.NewInt(4)
	
	h, _ := poseidon.HashWithWidth([]*big.Int{b1, b2, b3, b4, b5}, 5) 
	fmt.Println(fmt.Sprintf("%064s", h.Text(16)))
```
