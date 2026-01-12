usecaseDiagram
    actor "Khách hàng" as KH
    actor "Nhân viên" as NV
    actor "Quản lý" as QL

    rectangle "Hệ thống quản lý cửa hàng giày" {
        (Đăng nhập)
        (Xem giày)
        (Mua giày)
        (Bán giày)
        (Lập hóa đơn)
        (Quản lý giày)
        (Quản lý nhân viên)
        (Xem báo cáo)
    }

    KH --> (Xem giày)
    KH --> (Mua giày)

    NV --> (Đăng nhập)
    NV --> (Bán giày)
    NV --> (Lập hóa đơn)

    QL --> (Đăng nhập)
    QL --> (Quản lý giày)
    QL --> (Quản lý nhân viên)
    QL --> (Xem báo cáo)

    (Bán giày) --> (Lập hóa đơn) : <<include>>
