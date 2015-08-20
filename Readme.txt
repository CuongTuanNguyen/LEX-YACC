#Code demo phân tích từ vựng - ứng dụng thực hiện cộng, trừ, nhân, chia biểu thức
ví dụ 1+2(1+3)
chương trình phân tích và tính toán trả về kết quả bằng 9
#Cách tạo file thực thi từ file LEX và YACC
- 	Ta dùng công cụ flex để tạo ra các bộ kiểm tra nhằm nhận các mẫu
	từ vựng trong tập tin đầu vào được đặc tả theo tiêu chuẩn của lex
-	Dùng bison là một bộ phân tích cú pháp theo tiêu chuẩn đặc tả yacc
	giúp phát sinh tự động một chương trình xử lý tương ứng tập tin đầu vào
-	Dùng Dev-C để file thực thi
B1:	Ta copy 2 file calc.l và calc.y vào thư mục "GnuWin32\Bin" đã cài sẵn YACC và Flex
B2: Chạy Command Prompt truy xuất tới thư mục "GnuWin32\Bin"
	Thực thi file calc.y bằng lệnh "bison -d calc.y"
	Thực thi file clac.l bằng lệnh "flex calc.l"
B3: Sau khi thực thi 2 lệnh trên ta có được các file
	lex.yy.c và 2 file calc.tab.c, calc.tab.h 
	copy 3 file vào bin của dev-c tạo file thực thi bằng lệnh	
	"gcc calc.tab.c lex.yy.c -o calc.exe"