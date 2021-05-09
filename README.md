;# do.an.07

while True:
    thoigian = int(input("Nhập thời gian làm việc: ")) # nhập vào biến
    if(thoigian in range(8, 18)):         # cho biến chạy từ 8 ->17
        while True:
            name = input("Hãy Nhập tên: ") # nhập tên khách hàng 
            n = name.split(' ') # tạo khoảng cách cho từng phần của tên
            for i in range(len(n)): # cho i chạy trong độ dài của n
                if(not (n[i].isalpha()) or (n[i].isdigit())): # điều kiện không phải là số hoặc kí tự đặc biệt 
                    print("Hãy nhập lại:") # yêu cầu nhập lại
                    break # kết thúc vòng lập 
            else: # ngược lại
                print("Ho ten: ", ' '.join(n)) # xuất ra họ tên từ n
                break #kết thúc vòng lập while

        from datetime import  date
        def ntns():
            while True: 
                ngay = int(input("Nhập ngày sinh: "))# nhập ngày
                if (ngay not in range(1,32)): # điều kiện ngày phải từ khoảng 1 --->31
                    print("Mời nhập lại!") # yêu cầu nhập lại
                    continue # nếu nhập sai vòng lập tiếp tục cho tới khi đúng
                else: #khác
                    thang = int(input("Nhập tháng sinh: ")) # nhập tháng
                    if(thang not in range(1,13)): # điều kiện tháng phải thuộc khoảng 1--->12

                        print("Mời nhập lại tháng!") # nếu không thỏa điều kiện thì nhập lại tháng
                        continue # nếu sai thì tiếp tục nhập lại
                    else:
                        nam=int(input("Nhập năm sinh: ")) # nhập số năm
                        if (nam not in range (1900, 2022)): # điều kiện năm phải thuộc khoảng từ 1900--->2021
                            print("Mời nhập lại năm") #  nếu không thỏa điều kiện yêu cầu nhập lại
                            continue # nếu chưa thỏa thì tiếp tục nhập
                        else:
                            namsinh = ' Ngày tháng năm sinh: ' + str(ngay)+ '/'+str(thang)+'/'+str(nam)
                            return namsinh # ngày tháng năm khi xuất sẽ có thêm dấu "/" sau mỗi phần nhập
                            break # kết thúc vòng lập while

        a = ntns()
        print(a) # xuất ra ngày tháng năm
        while True:
            n = input("Nhập mã tài khoản khách hàng: ") # nhập tài khoảng

            if ((len(n) > 12) or (len(n) < 12)): # nếu độ dài của n > 12 hoặc <12 
                print("---Vui lòng nhập lại---") # yêu cầu nhập lại
            else:
                print(f"Tài khoản là: {n}") # xuất ra tài khoảng
                break #kết thúc vòng lập wwhile

        while True:
            c = input("Nhập số căn cước công dân: ") # nhập số căn cước công dân
            if (len(c) > 12 or len(c) <12): # nếu độ dài của n > 12 hoặc <12 
                print("---Vui lòng nhập lại---") # yêu cầu nhập lại
            else:
                print(f"Số căn cước là : {c}") # xuất ra số căn cước
                break # kết thúc vòng lập while

        while True:
            v = input("Nhập Số Điện Thoại: ") # nhập số điện thoại
            if (len(v) > 10 or len(v) < 10):#nếu độ dài của n > 9 hoặc < 9
                print("---Vui lòng nhập lại---") # yêu cầu nhập lại
            else:
                print(f"Số Điện Thoại:{v}") # xuất ra số điện thoại
                break # kết thúc vòng lập while

        while True:
            k = int(input("Nhập số dư tài khoản: ")) # nhập số dư tài khoản
            if k > 100000000000: # Nếu số tiền dư trong tài khoản lớn hơn 100 tỉ
                print ("Số tiền quá mức") # in ra : số tiền quá mức
            else:
                print(f"Số dư tài khoản là: {k}") # ngược lại sẽ in ra số dư tài khoản và k
                sodu = int(k) # đặt biến của số dư tài khoản 
                break # nếu đúng thì dừng lại 
        print("Họ tên:", name) # in ra tên họ tên của khách hàng
        print(a) # in ra ngày tháng năm sinh của khách hàng 
        print("Số điện thoại: ", v) # in ra số điện thoại của khách hàng
        print("Số dư tài khoản là: ", k, "đồng") # in ra số dư tài khoản của khách hàng kèm theo đơn vị là " Đồng"
        #-------------------------------------------------------------------------------

        giasan_A = 4200 
        giatran_A = 2000 
        giasan_B = 5300 
        giatran_B = 3000
        giasan_C = 5000 
        giatran_C = 3600 

        chungkhoan = ["A", "B", "C"] # danh sách mã số cổ phiếu
        list1 = [] # tạo danh sách rỗng

        print ("Mời mua cổ phiếu: ") # in số cổ phiếu 
        for i in range(len(chungkhoan)): #  cho i chạy qua độ dài của biến chạy từ 0 ->3  
            print('-'*20) # in ra - x20 lần
            print ("---------MÃ CỔ PHIẾU A------------") # in ra mã cổ phiếu A
            print("Gía sàn A:", giasan_A, "VND") #  in ra giá sàn A kèm theo đơn vị là VND
            print("Giá trần A:", giatran_A, "VND") # in ra giá trần A kèm theo đơn vị là VND
            print ("---------MÃ CỔ PHIẾU B------------") # in ra mã cổ phi
            print("Gía sàn B:", giasan_B, "VND") # in ra giá sàn B kèm theo đơn vị là VND
            print("Giá trần B:", giatran_B, "VND") # in ra giá trần B kèm theo đơn vị là VND
            print ("---------MÃ CỔ PHIẾU C------------") # n ra mã cổ phiếu C
            print("Gía sàn C:", giasan_C, "VND") # in ra giá sàn C kèm theo đơn vị là VND
            print("Giá trần C:", giatran_C, "VND") # in ra giá trần C kèm theo đơn vị là VND
            break # kết thúc vòng lập for 
            list1.append(giasan) # đưa biến giasan vào danh sách list 1
            list1.append(giatran) # đưa biến giatran vào danh sách list 1


        for j in range(len(chungkhoan)): #  cho j chạy qua đọ dài của biến chạy từ 0->3
            if(chungkhoan[j] == "A"): # Nếu j bằng A
                nhap2 = input("Chọn cổ phiếu A (S1/T1): ") # 
                if(nhap2 == "S1"): # Nếu nhap2 bằng S1
                    print(f"Gía sàn: {giasan_A}") # in ra gía sàn 
                    value1 = int(giasan_A) # chuyển giasan_A về hệ số nguyên vào giá trị value 1
                elif(nhap2 == "T1"): # nếu nhap 2 = T1
                    print(f"Gía trần: {giatran_A}") # in ra giá trần 
                    value1 = int(giatran_A) # chuyển giatran_A về hệ số nguyên vào giá trị value1 

            elif(chungkhoan[j] == "B"): # Nếu chungkhoan J bằng B
                nhap3 = input("Chọn cổ phiếu B (S2/T2): ") # xuất ra chọn cổ phiếu B
                if(nhap3 == "S2"): # Nếu nhap3 bằng s2
                    print(f"Gía sàn: {giasan_B}") # in ra giá sàn 
                    value2 = int(giasan_B) # chuyển giasan_B về hệ số nguyên vào giá trị value 2 
                elif(nhap3 == "T2"): # Nếu nhap3 bằng T2
                    print(f"Gía trần: {giatran_B}") # in ra giá trần
                    value2 = int(giatran_B) # chuyển giatran_B về hệ số nguyên vào giá trị value2 
            else:
                nhap4 = input("Chọn cổ phiếu C (S3/T3): ") # Xuất ra chọn cổ phiếu 
                if(nhap4 == "S3"): # nếu nhap4 bằng S3
                    print(f"Gía sàn: {giasan_C}") # in ra giá sàn 
                    value3 = int(giasan_C) # chuyển giasan_C về hệ số nguyên vào giá trị value 3
                elif(nhap4 == "T3"): # Nếu nhap 4 bằng T3
                    print(f"Gía trần: {giatran_C}") # in ra giá trần 
                    value3 = int(giatran_C) # chuyển giatran_C về hệ số nguyên vào giá trị value 3
                    print ("-----------------------------")
                    break

       

        math = value1 + value2 + value3 # tính tổng giá trần giá sàn

        print ("Số tiền là:", value1, "đồng ;" ,value2, "đồng ;" ,value3, "đồng ;") # in ra số tiền của từng mã cổ phiếu kèm theo đơn vị là "đồng" 
        print ("Tổng cộng là: ", math, "đồng") # in ra tổng tiền
        print ("--------------=&=---------------")

        if sodu > math: # nếu sodu lớn hơn math
            print ("Bạn có đủ tiền để mua cổ phiếu") 
            print ("-------------------------------")
            break
        else:
                print("Bạn không có đủ tiền. Hãy thử lại.")
                print ("----------------------------------")
                break
    else: 
        print("Chỉ có thế làm việc từ: 8h - 17h")
        break


