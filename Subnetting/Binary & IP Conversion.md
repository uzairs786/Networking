# 🔢 Binary & IP Conversion

---

## 🌍 Why Binary Matters
- Computers don’t understand decimal (0–9), they understand **binary (0s & 1s)**.  
- Networking (IP addresses, subnetting, routing) is built on binary.  
- Mastering binary = understanding how networks actually work ⚡.

---

## 🧮 Binary Basics
- **Binary** = Base 2 (only uses `0` and `1`).  
- Each digit = **bit**.  
- Bits represent **powers of 2**, starting from the right:  

```

Binary: 101010
Decimal: (1×2⁵) + (0×2⁴) + (1×2³) + (0×2²) + (1×2¹) + (0×2⁰)
= 32 + 0 + 8 + 0 + 2 + 0
= **42**

```

✅ `101010 (binary)` → `42 (decimal)`

---

## 🌐 IP Addresses in Binary
- An IPv4 address = **4 octets** (each 8 bits).  
- Example: `192.168.1.1`

### Step 1 – Convert 192
- Divide by 2, keep remainders:  
192 ÷ 2 = 96 R0  
96 ÷ 2 = 48 R0  
48 ÷ 2 = 24 R0  
24 ÷ 2 = 12 R0  
12 ÷ 2 = 6 R0  
6 ÷ 2 = 3 R0  
3 ÷ 2 = 1 R1  
1 ÷ 2 = 0 R1  

Read **remainders in reverse** → `11000000`  

✅ 192 → `11000000`

---

### Step 2 – Convert 168
168 → `10101000`

---

### Step 3 – Convert 1
1 → `00000001`

---

### ✅ Final Binary Form
`192.168.1.1` =  
`11000000.10101000.00000001.00000001`

---

## 📝 Practice Example
Convert these:

1. `10.0.0.1`  
   → `00001010.00000000.00000000.00000001`

2. `255.0.0.0` (Subnet Mask)  
   → `11111111.00000000.00000000.00000000`

---

## ⚡ Recap
- Binary = base 2 (powers of 2).  
- Decimal ↔ Binary conversion is key to subnetting.  
- IPv4 = 32 bits = 4 × 8-bit octets.  

