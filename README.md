**ZERO2HER**
Hướng dẫn chạy Blockmesh trên vps

👉 Link BlockMesh : [Click](https://app.blockmesh.xyz/register?invite_code=f516e268-9595-4ca6-ad15-30ba652a890d)

Anh em cài screen để quản lí các tool cho dễ, cứ 1 kèo thì ném vào screen riêng

Đầu tiên cài screen trước

sudo apt install screen
sau đó tạo 1 phiên screen bằng lệnh

screen -S blockmesh
Bắt đầu cài đặt và chạy blockmesh, chạy lệnh bên dưới

wget -O blockmesh.sh https://raw.githubusercontent.com/phuctranduy2/blockmesh/refs/heads/main/blockmesh.sh && chmod +x blockmesh.sh && ./blockmesh.sh
Đến bước điền tài khoản mật khẩu thì điền tài khoản blockmesh vào là được (đã xác minh gmail)

Kiểm tra log bằng lệnh

docker logs -f blockmesh-cli-container
anh em muốn vào lại phiên thì dùng

screen -r blockmesh
thoát phiên dùng tổ hợp phím ctrl + a rồi d (google cho chi tiết các lệnh)
