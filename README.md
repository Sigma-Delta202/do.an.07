# do.an.07
while True:
    thoigian = int(input("Nhập thời gian làm việc: "))
    if(thoigian in range(8, 18)):        
        while True:
            name = input("Hãy Nhập tên: ") # nhập tên khách hàng 
            n = name.split(' ') # tạo khoảng cách cho từng phần của tên
            for i in range(len(n)): #tạo vòng lập cho n
                if(not (n[i].isalpha()) or (n[i].isdigit())): # điều kiện không phải là chữ hoặc số/kí tự 
                    print("Hãy nhập lại:") # yêu cầu nhập lại
                    break # kết thúc vòng lập 
            else: # ngược lại
                print("Ho ten: ", ' '.join(n)) # xuất ra họ tên từ n
                break #kết thcs vòng lập while

        from datetime import  date
        def ntns():
            while True: 
                ngay = int(input("Nhập ngày sinh: "))# nhập ngày
                if (ngay not in range(1,32)): # điều kiện nếu ngày không phải từ khoảng 1 --->32
                    print("Mời nhập lại!") # yêu cầu nhập lại
                    continue # nếu nhập sai vòng lập tiếp tuc cho tới khi đúng
                else: #khác
                    thang = int(input("Nhập tháng sinh: ")) # nhập tháng
                    if(thang not in range(1,13)): # điều kiện nếu tháng không thuộc khoảng 1--->13

                        print("Mời nhập lại tháng!") # nếu không thỏa điều kiện thì nhập lại tháng
                        continue # nếu sai thì tiếp tục nhập lại
                    else:
                        nam=int(input("Nhập năm sinh: ")) # nhập số năm
                        if (nam not in range (1900, 2021)): # điều kiện nếu năm không thuộc khoảng từ 1900--->2021
                            print("Mời nhập lại năm") #  nếu không thỏa điều kiện yêu cầu nhập lại
                            continue # ếu chưa thỏa thì tiếp tục nhập
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
            k = int(input("Nhập số dư tài khoản: "))
            if k > 100000000000:
                print ("Số tiền quá mức")
            else:
                print(f"Số dư tài khoản là: {k}")
                sodu = int(k)
                break
        print ("-----------------*----------------")
        print(name)
        print(a)
        print(v)
        print(k)
        print ("-----------------*----------------")
        print ("-----------------&----------------")
        #-------------------------------------------------------------------------------

        giasan_A = 4200 
        giatran_A = 2000 
        giasan_B = 5300 
        giatran_B = 3000
        giasan_C = 5000 
        giatran_C = 3600 

        chungkhoan = ["A", "B", "C"]
        list1 = []

        print ("Mời mua cổ phiếu: ")
        for i in range(len(chungkhoan)):
            print('-'*20)
            print ("---------MÃ CỔ PHIẾU A------------")
            print("Gía sàn A:", giasan_A, "VND")
            print("Giá trần A:", giatran_A, "VND")
            print ("---------MÃ CỔ PHIẾU B------------")
            print("Gía sàn B:", giasan_B, "VND")
            print("Giá trần B:", giatran_B, "VND")
            print ("---------MÃ CỔ PHIẾU C------------")
            print("Gía sàn C:", giasan_C, "VND")
            print("Giá trần C:", giatran_C, "VND")
            break
            list1.append(giasan)
            list1.append(giatran)


        for j in range(len(chungkhoan)):
            if(chungkhoan[j] == "A"):
                nhap2 = input("Chọn cổ phiếu A (S1/T1): ")
                if(nhap2 == "S1"):
                    print(f"Gía sàn: {giasan_A}")
                    value1 = int(giasan_A)
                elif(nhap2 == "T1"):
                    print(f"Gía trần: {giatran_A}")
                    value1 = int(giatran_A)

            elif(chungkhoan[j] == "B"):
                nhap3 = input("Chọn cổ phiếu B (S2/T2): ")
                if(nhap3 == "S2"):
                    print(f"Gía sàn: {giasan_B}")
                    value2 = int(giasan_B)
                elif(nhap3 == "T2"):
                    print(f"Gía trần: {giatran_B}")
                    value2 = int(giatran_B)
            else:
                nhap4 = input("Chọn cổ phiếu C (S3/T3): ")
                if(nhap4 == "S3"):
                    print(f"Gía sàn: {giasan_C}")
                    value3 = int(giasan_C)
                elif(nhap4 == "T3"):
                    print(f"Gía trần: {giatran_C}")
                    value3 = int(giatran_C)
                    print ("-----------------------------")
                    break

        math = value1 + value2 + value3

        print ("Số tiền là:", value1, "đồng ;" ,value2, "đồng ;" ,value3, "đồng ;")
        print ("Tổng cộng là: ", math, "đồng")
        print ("--------------=&=---------------")

        if sodu > math:
            print ("Bạn có đủ tiền để mua cổ phiếu")
            print ("-------------------------------")
        else:
                print("Bạn không có đủ tiền. Hãy thử lại.")
                print ("----------------------------------")

        math = value1 + value2 + value3

        print ("Số tiền là:", value1, "đồng ;" ,value2, "đồng ;" ,value3, "đồng ;")
        print ("Tổng cộng là: ", math, "đồng")
        print ("--------------=&=---------------")

        if sodu > math:
            print ("Bạn có đủ tiền để mua cổ phiếu")
            print ("-------------------------------")
        else:
                print("Bạn không có đủ tiền. Hãy thử lại.")
                print ("----------------------------------")

    else: 
        print("Chỉ có thế làm việc từ: 8h - 17h")
        break
