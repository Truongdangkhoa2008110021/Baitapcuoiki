/*
*Ngày tạo : 29 thg 11, 2021
*Tác giả : Trương Đăng Khoa
*/
package com.Khoatd2008110021.BaiKiemTraCuoiKi;

import java.sql.Date;
import java.text.DecimalFormat;
import java.text.ParseException;
import java.util.Scanner;

public class SanhSu extends HangHoa {
   
    private String noiSanXuat;

    public SanhSu(String tenHangHoa, String maHH, long donGia, String ngayNhapKho, int soLuongTonKho,
            String noiSanXuat) throws ParseException {
        super("HSS-"+tenHangHoa, maHH, donGia, ngayNhapKho, soLuongTonKho);
        this.noiSanXuat = noiSanXuat;
    }

    public String getNoiSanXuat() {
        return noiSanXuat;
    }

    public void setNoiSanXuat(String noiSanXuat) {
        this.noiSanXuat = noiSanXuat;
    }

    DecimalFormat ft = new DecimalFormat("###,###,### VND");

    @Override
    public String toString() {
        return "SanhSu [ft=" + ft + ", noiSanXuat=" + noiSanXuat + "]";
    }    
}
