Khoa(maKhoa*, tenKhoa, maIn) *DV_xxxx          
BoMon(maBoMon*, maKhoa, tenBoMon, maIn) *BM_xxxx
GiaoVien(maGiaoVien*, maIn, maBoMon, tenGiaoVien, queQuan, gioiTinh, ngaySinh, thangSinh, namSinh, ngayBatDau, ngayKetThuc) *GV_xxxx
ThanNhan(maThanNhan*, maIn, tenThanNhan, ngaySinh, gioiTinh, ngheNghiep) *TN_xxxx
GiaoVien_ThanNhan(maGV*, maThanNhan*)
DiaChiLienHe(maLienHe*, phuong, quan, thanhPho, dienThoaiNhaRieng, dienThoaiDiDong, email)
LichSuDiaChiLienHe(maGiaoVien*, maLienHe, namBatDau, namKetThuc)


MienGiam(maMienGiam*, maIn, tyLeMienGiam) *MG_xxxx

ChucVuDang(maChucVuDang*, maMienGiam, tenChucVuDang) *CVD_xxxx

ChucVuChinhQuyen(maChucVuChinhQuyen*, maMienGiam, tenChucVuChinhQuyen) *CVCQ_xxxx

ChucVuChuyenMonNghiepVu(maChucVuChuyenMonNghiepVu*, maDinhMucDaoTao, maDinhMucNghienCuu, tenChucVuChuyenMonNghiepVu)

HoSoChucVuDang(maHoSoChucVuDang*, maIn, maGiaoVien, maChucVuDang, thoiDiemMãNhan, thoiDiemKetThuc) *HSCVD_xxxx

HoSoHocVan(maHoSoHocVan*, maIn, maGiaoVien, maHocVan, thoiDiemNhan, thoiDiemKetThuc) *HSHV_xxxx
HoSoHocHam(maHoSoHocHam*, maIn, maGiaoVien, maHocHam, thoiDiemNhan, thoiDiemKetThuc) *HSHH_xxxx 
HSCVCMNV ????

HocHam(maHocHam*, maDinhMucDaoTao, maDinhMucNghienCuu, tenHocHam)
HocVi(maHocVi*, tenHocVi) *HVi_xxxx
HocVan(maHocVan*, maIn, maHocVi, tenTrinhDo, nuocDaoTao, heDaoTao, noiDaoTao, namCap, tenLuanAn) *HVan_xxxx
DinhMucDaoTao(maDinhMucDaoTao*, tenDinhMuc, soGioDinhMucDaoTao, soGioDinhMucDaoTaoQuocPhong) 
DinhMucNghienCuu(maDinhMucNghienCuu*, tenDinhMuc, soGioDinhMucNghienCuu, gioChuanDinhMucNghienCuu)

HocPhan(maHocPhan*, tenHocPhan, maBoMon, soTiet, soTinChi) *HP_xxxx
Lop(maLop*, maHocPhan, tenLop, he, siSo, hocKy, namHoc) *Lop_xxxx

CongViecGiangDay(maCongViecGiangDay*, maIn, maGioChuanGiangDay, maLop) *CVGD_xxxx
GioChuanGiangDay(maGioChuanGiangDay, tenGioChuan, soGio, donVi,so)
PhanCongGiangDay(maGiaoVien*, maCongViecGiangDay*, soTietDay, hocKyBatDau*, namHocBatDau*)

GioChuanHoiDong(maGioChuanHoiDong, tenGioChuan, soGio, donVi, so)
CongViecHoiDong(maCongViecHoiDong*, maIn, maGioChuanHoiDong, tenHoiDong) *CVHD_xxxx
VaiTroHoiDong(maVaiTroHoiDong*, tenVaiTro)
PhanCongHoiDong(maGiaoVien*, maCongViecHoiDong*, maVaiTroHoiDong*,soLan,  hocKy, namHoc)

GioChuanHuongDan(maGioChuanHuongDan*, maIn, tenGioChuan, soGio, donVi,so) 
CongViecHuongDan(maCongViecHuongDan*, maIn, maGioChuanHuongDan) *CVHD_xxxx
PhanCongHuongDan(maGiaoVien*, maCongViecHuongDan*)
HuongDanHocVien(maHuongDanHocVien*, maCongViecHuongDan, maHocVien, tenDeTai)

HocVienLop(maHocVien*, maLop*)
HocVien(maHocVien*, maIn, tenHocVien) *HV_xxxx 


CongViecKhaoThi(maCongViecKhaoThi*, maIn, maGioChuanKhaoThi, maLop) *CVKT_xxxx
GioChuanKhaoThi(maGioChuanKhaoThi, tenGioChuan, soGio, donVi, so)
PhanCongKhaoThi(maGiaoVien*, maCongViecKhaoThi*, SoBai, MaHocPhan*, hocKyBatDau*, namHocBatDau*)



DonViTinh(maDonViTinh*, donVi, so)
LoaiNghienCuu(maLoaiNghienCuu*, tenLoaiNghienCuu)
VaiTro(maVaiTro*, maLoaiNghienCuu, tenVaiTro)

LoaiCongTrinh(maLoaiCongTrinh*, tenLoaiCongTrinh, gioChuan) 
CongTrinhKhoaHoc(maCongTrinhKhoaHoc*, maLoaiCongTrinh, maLoaiNghienCuu, maDonViTinh, tenCongTrinh, soTacGia) *CTKH_xxxx
PhanCongNghienCuu(maGiaoVien*, maCongTrinhKhoaHoc*, maVaiTro, hocKyBatDau*, namHocBatDau*, hocKyKetThuc, namHocKetThuc)



ThuocTinh(maThuocTinh, tenThuocTinh) ???? 
LoaiNghienCuuThuocTinh(maLoaiNghienCuu*, maThuocTinh*, noiDung ) ????