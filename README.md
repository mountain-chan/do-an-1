# do-an-1
Đề tài: Xây dựng dịch vụ chat an toàn với RSA

## Đồng dư là gì.
Cho số nguyên dương n, hai số nguyên: a,b được gọi là đồng dư theo mô-đun n nếu chúng có cùng số dư khi chia cho n. Điều này tương đương với hiệu a-b chia hết cho n.

# RSA 

## Tạo mã
•	Chọn một số tự nhiên **e** trong khoảng **(1, λ(n)) sao cho ƯCLN(e, λ(n)) = 1**, tức là e và λ(n) nguyên tố cùng nhau.

•	Tính toán số d sao cho **de ≡ 1 mod λ(n)**. Số d được gọi là số nghịch đảo mô-đun của e (theo mô-đun mod λ(n)).

•	Public key sẽ là bộ số (n, e), và private key sẽ là bộ số (n, d).

## Mã hoá và giải mã
Giả sử m là tin nhắn cần mã hoá, c là tin nhắn đã được mã hoá.

### Mã hoá
**c ≡ m^e mod n**

### Giải mã
**c^d ≡ m^de ≡ m mod n => m = c^d % n**
